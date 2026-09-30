---
title: "SevenZipArchive.CreateEntry"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "SevenZipArchive メソッド。アーカイブ内に単一のエントリを作成します"
type: docs
weight: 50
url: /ja/net/aspose.zip.sevenzip/sevenziparchive/createentry/
---
## CreateEntry(string, FileInfo, bool, SevenZipEntrySettings) {#createentry_1}

アーカイブ内に単一のエントリを作成します。

```csharp
public SevenZipArchiveEntry CreateEntry(string name, FileInfo fileInfo, 
    bool openImmediately = false, SevenZipEntrySettings newEntrySettings = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| name | String | エントリの名前。 |
| fileInfo | FileInfo | 圧縮するファイルのメタデータ。 |
| openImmediately | Boolean | ファイルをすぐに開く場合は True、そうでなければアーカイブ保存時にファイルを開きます。 |
| newEntrySettings | SevenZipEntrySettings | 追加された [`SevenZipArchiveEntry`](../../sevenziparchiveentry/) アイテムに使用される圧縮および暗号化設定です。個別の圧縮設定はソリッド圧縮の場合は無視されます。詳細は [`Solid`](../../../aspose.zip.saving/sevenzipentrysettings/solid/) を参照してください。 |

### 戻り値

Seven Zip エントリ インスタンスです。

### 例外

| 例外 | 条件 |
| --- | --- |
| UnauthorizedAccessException | *fileInfo* は読み取り専用か、ディレクトリです。 |
| ArgumentException | *name* が null または空です。 |
| DirectoryNotFoundException | 指定されたパスが無効です（例: マッピングされていないドライブ上にある場合）。 |
| IOException | ファイルは既に開かれています。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |

## 備考

エントリ名は *name* パラメータ内でのみ設定されます。*fileInfo* パラメータで指定されたファイル名はエントリ名に影響しません。

*openImmediately* パラメータでファイルをすぐに開くと、アーカイブが保存されるまでブロックされます。

## 例

各エントリが異なるパスワードで暗号化されたアーカイブを作成します。

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    FileInfo fi1 = new FileInfo("data1.bin");
    FileInfo fi2 = new FileInfo("data2.bin");
    FileInfo fi3 = new FileInfo("data3.bin");
    using (var archive = new SevenZipArchive())
    {
        archive.CreateEntry("entry1.bin", fi1, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test1")));
        archive.CreateEntry("entry2.bin", fi2, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test2")));
        archive.CreateEntry("entry3.bin", fi3, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test3")));
        archive.Save(sevenZipFile);
    }
}
```

### 関連項目

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, SevenZipEntrySettings, FileSystemInfo) {#createentry_3}

アーカイブ内に単一のエントリを作成します。

```csharp
public SevenZipArchiveEntry CreateEntry(string name, Stream source, 
    SevenZipEntrySettings newEntrySettings, FileSystemInfo fileInfo)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| name | String | エントリの名前。 |
| source | Stream | エントリの入力ストリーム。 |
| newEntrySettings | SevenZipEntrySettings | 追加された [`SevenZipArchiveEntry`](../../sevenziparchiveentry/) アイテムに使用される圧縮および暗号化設定です。個別の圧縮設定はソリッド圧縮の場合は無視されます。詳細は [`Solid`](../../../aspose.zip.saving/sevenzipentrysettings/solid/) を参照してください。 |
| fileInfo | FileSystemInfo | 圧縮するファイルまたはフォルダーのメタデータ。 |

### 戻り値

SevenZip エントリ インスタンスです。

### 例外

| 例外 | 条件 |
| --- | --- |
| InvalidOperationException | *source* と *fileInfo* の両方が null であるか、*source* が null で *fileInfo* がディレクトリを表す場合です。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |
| ArgumentException | *name* が null または空です。 |

## 備考

エントリ名は *name* パラメータ内でのみ設定されます。*fileInfo* パラメータで指定されたファイル名はエントリ名に影響しません。

*fileInfo* can refer to DirectoryInfo if the entry is directory.

## 例

LZMA2 圧縮かつ暗号化されたエントリを含むアーカイブを作成します。

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive())
    {
        archive.CreateEntry("entry1.bin", new MemoryStream(new byte[] {0x00, 0xFF}), new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings(), new SevenZipAESEncryptionSettings("test1")), new FileInfo("data1.bin")); 
        archive.Save(sevenZipFile);
    }
}
```

### 関連項目

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Func&lt;Stream&gt;, SevenZipEntrySettings) {#createentry}

アーカイブ内に単一のエントリを作成します。

```csharp
public SevenZipArchiveEntry CreateEntry(string name, Func<Stream> streamProvider, 
    SevenZipEntrySettings newEntrySettings = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| name | String | エントリの名前。 |
| streamProvider | Func`1 | エントリ用の入力ストリームを提供するメソッドです。 |
| newEntrySettings | SevenZipEntrySettings | 追加された [`SevenZipArchiveEntry`](../../sevenziparchiveentry/) アイテムに使用される圧縮および暗号化設定です。個別の圧縮設定はソリッド圧縮の場合は無視されます。詳細は [`Solid`](../../../aspose.zip.saving/sevenzipentrysettings/solid/) を参照してください。 |

### 戻り値

SevenZip エントリ インスタンスです。

### 例外

| 例外 | 条件 |
| --- | --- |
| InvalidOperationException | アーカイブは解凍用にインスタンス化されています |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |
| ArgumentException | *name* が null または空です。 |

## 例

LZMA2 圧縮かつ暗号化されたエントリを含むアーカイブを作成します。

```csharp
System.Func<Stream> provider = delegate(){ return new MemoryStream(new byte[]{0xFF, 0x00}); };
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive())
    {
        archive.CreateEntry("entry1.bin", provider, new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings(), new SevenZipAESEncryptionSettings("test1"))); 
        archive.Save(sevenZipFile);
    }
}
```

### 関連項目

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, SevenZipEntrySettings) {#createentry_2}

アーカイブ内に単一のエントリを作成します。

```csharp
public SevenZipArchiveEntry CreateEntry(string name, Stream source, 
    SevenZipEntrySettings newEntrySettings = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| name | String | エントリの名前。 |
| source | Stream | エントリの入力ストリーム。 |
| newEntrySettings | SevenZipEntrySettings | 追加された [`SevenZipArchiveEntry`](../../sevenziparchiveentry/) アイテムに使用される圧縮および暗号化設定です。個別の圧縮設定はソリッド圧縮の場合は無視されます。詳細は [`Solid`](../../../aspose.zip.saving/sevenzipentrysettings/solid/) を参照してください。 |

### 戻り値

Zip エントリ インスタンス。

### 例外

| 例外 | 条件 |
| --- | --- |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |
| ArgumentException | *name* が null または空です。 |

## 例

すべてのエントリを LZMA2 圧縮および暗号化した 7z アーカイブを作成します。

```csharp
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings(), new SevenZipAESEncryptionSettings("p@s$"))))
{
    archive.CreateEntry("data.bin", new MemoryStream(new byte[] {0x00, 0xFF} ));
    archive.Save("archive.7z");
}
```

### 関連項目

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool, SevenZipEntrySettings) {#createentry_4}

アーカイブ内に単一のエントリを作成します。

```csharp
public SevenZipArchiveEntry CreateEntry(string name, string path, bool openImmediately = false, 
    SevenZipEntrySettings newEntrySettings = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| name | String | エントリの名前。 |
| path | String | 新しいファイルの完全修飾名、または圧縮対象の相対ファイル名。 |
| openImmediately | Boolean | ファイルをすぐに開く場合は True、そうでなければアーカイブ保存時にファイルを開きます。 |
| newEntrySettings | SevenZipEntrySettings | 追加された [`SevenZipArchiveEntry`](../../sevenziparchiveentry/) アイテムに使用される圧縮および暗号化設定です。個別の圧縮設定はソリッド圧縮の場合は無視されます。詳細は [`Solid`](../../../aspose.zip.saving/sevenzipentrysettings/solid/) を参照してください。 |

### 戻り値

Zip エントリ インスタンス。

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *path* が null です。 |
| SecurityException | 呼び出し元にはアクセスに必要な権限がありません。 |
| ArgumentException | *path* が空、または空白文字のみ、または無効な文字が含まれています。 - または - *name* が null または空です。 |
| UnauthorizedAccessException | ファイル *path* へのアクセスが拒否されました。 |
| PathTooLongException | 指定された *path*、ファイル名、またはその両方がシステム定義の最大長を超えています。例として、Windows ベースのプラットフォームでは、パスは 248 文字未満、ファイル名は 260 文字未満である必要があります。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |
| NotSupportedException | *path* のファイル名に文字列の途中にコロン (:) が含まれています。 |

## 備考

エントリ名は *name* パラメータ内でのみ設定されます。*path* パラメータで指定されたファイル名はエントリ名に影響しません。

*openImmediately* パラメータでファイルをすぐに開くと、アーカイブが保存されるまでブロックされます。

## 例

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings())))
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(sevenZipFile);
    }
}
```

### 関連項目

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)


