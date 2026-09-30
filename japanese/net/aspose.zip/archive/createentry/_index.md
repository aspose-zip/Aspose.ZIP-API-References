---
title: "Archive.CreateEntry"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Archive メソッド。アーカイブ内に単一のエントリを作成します"
type: docs
weight: 60
url: /ja/net/aspose.zip/archive/createentry/
---
## CreateEntry(string, string, bool, ArchiveEntrySettings) {#createentry_4}

アーカイブ内に単一のエントリを作成します。

```csharp
public ArchiveEntry CreateEntry(string name, string path, bool openImmediately = false, 
    ArchiveEntrySettings newEntrySettings = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| name | String | エントリの名前。 |
| path | String | 新しいファイルの完全修飾名、または圧縮対象の相対ファイル名。 |
| openImmediately | Boolean | ファイルをすぐに開く場合は True、そうでなければアーカイブ保存時にファイルを開きます。 |
| newEntrySettings | ArchiveEntrySettings | 追加された [`ArchiveEntry`](../../archiveentry/) アイテムに使用される圧縮および暗号化設定。 |

### 戻り値

Zip エントリ インスタンス。

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *path* が null です。 |
| SecurityException | 呼び出し元にはアクセスに必要な権限がありません。 |
| ArgumentException | *path* が空であるか、空白文字のみ、または無効な文字が含まれています。 |
| UnauthorizedAccessException | ファイル *path* へのアクセスが拒否されました。 |
| PathTooLongException | 指定された *path*、ファイル名、またはその両方がシステム定義の最大長を超えています。例として、Windows ベースのプラットフォームでは、パスは 248 文字未満、ファイル名は 260 文字未満である必要があります。 |
| NotSupportedException | *path* のファイル名に文字列の途中にコロン (:) が含まれています。 |
| ObjectDisposedException | アーカイブが破棄された場合にスローされます。 |

## 備考

エントリ名は *name* パラメータ内でのみ設定されます。*path* パラメータで指定されたファイル名はエントリ名に影響しません。

*openImmediately* パラメータでファイルをすぐに開くと、アーカイブが保存されるまでブロックされます。

## 例

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(zipFile);
    }
}
```

### 関連項目

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, ArchiveEntrySettings) {#createentry_2}

アーカイブ内に単一のエントリを作成します。

```csharp
public ArchiveEntry CreateEntry(string name, Stream source, 
    ArchiveEntrySettings newEntrySettings = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| name | String | エントリの名前。 |
| source | Stream | エントリの入力ストリーム。 |
| newEntrySettings | ArchiveEntrySettings | 追加された [`ArchiveEntry`](../../archiveentry/) アイテムに使用される圧縮および暗号化設定。 |

### 戻り値

Zip エントリ インスタンス。

### 例外

| 例外 | 条件 |
| --- | --- |
| ObjectDisposedException | アーカイブが破棄された場合にスローされます。 |
| InvalidOperationException | アーカイブの現在の状態によりエントリの追加が無効な場合にスローされます。 |

## 例

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new AesEcryptionSettings("p@s$", EncryptionMethod.AES256))))
{
    archive.CreateEntry("data.bin", new MemoryStream(new byte[] {0x00, 0xFF} ));
    archive.Save("archive.zip");
}
```

### 関連項目

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool, ArchiveEntrySettings) {#createentry_1}

アーカイブ内に単一のエントリを作成します。

```csharp
public ArchiveEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false, 
    ArchiveEntrySettings newEntrySettings = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| name | String | エントリの名前。 |
| fileInfo | FileInfo | 圧縮するファイルのメタデータ。 |
| openImmediately | Boolean | ファイルをすぐに開く場合は True、そうでなければアーカイブ保存時にファイルを開きます。 |
| newEntrySettings | ArchiveEntrySettings | 追加された [`ArchiveEntry`](../../archiveentry/) アイテムに使用される圧縮および暗号化設定。 |

### 戻り値

Zip エントリ インスタンス。

### 例外

| 例外 | 条件 |
| --- | --- |
| UnauthorizedAccessException | *fileInfo* は読み取り専用か、ディレクトリです。 |
| DirectoryNotFoundException | 指定されたパスが無効です（例: マッピングされていないドライブ上にある場合）。 |
| IOException | ファイルは既に開かれています。 |
| ObjectDisposedException | アーカイブが破棄された場合にスローされます。 |
| InvalidOperationException | アーカイブの現在の状態によりエントリの追加が無効な場合にスローされます。 |

## 備考

エントリ名は *name* パラメータ内でのみ設定されます。*fileInfo* パラメータで指定されたファイル名はエントリ名に影響しません。

*openImmediately* パラメータでファイルをすぐに開くと、アーカイブが保存されるまでブロックされます。

## 例

各エントリを異なる暗号化方式とパスワードで暗号化したアーカイブを作成します。

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    FileInfo fi1 = new FileInfo("data1.bin");
    FileInfo fi2 = new FileInfo("data2.bin");
    FileInfo fi3 = new FileInfo("data3.bin");
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry1.bin", fi1, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")));
        archive.CreateEntry("entry2.bin", fi2, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEcryptionSettings("pass2", EncryptionMethod.AES128)));
        archive.CreateEntry("entry3.bin", fi3, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEcryptionSettings("pass3", EncryptionMethod.AES256)));
        archive.Save(zipFile);
    }
}
```

### 関連項目

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, ArchiveEntrySettings, FileSystemInfo) {#createentry_3}

アーカイブ内に単一のエントリを作成します。

```csharp
public ArchiveEntry CreateEntry(string name, Stream source, ArchiveEntrySettings newEntrySettings, 
    FileSystemInfo fileInfo)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| name | String | エントリの名前。 |
| source | Stream | エントリの入力ストリーム。 |
| newEntrySettings | ArchiveEntrySettings | 追加された [`ArchiveEntry`](../../archiveentry/) アイテムに使用される圧縮および暗号化設定。 |
| fileInfo | FileSystemInfo | 圧縮するファイルまたはフォルダーのメタデータ。 |

### 戻り値

Zip エントリ インスタンス。

### 例外

| 例外 | 条件 |
| --- | --- |
| InvalidOperationException | *source* と *fileInfo* の両方が null であるか、*source* が null で *fileInfo* がディレクトリを表す場合です。 |
| ObjectDisposedException | アーカイブが破棄された場合にスローされます。 |

## 備考

エントリ名は *name* パラメータ内でのみ設定されます。*fileInfo* パラメータで指定されたファイル名はエントリ名に影響しません。

*fileInfo* can refer to DirectoryInfo if the entry is directory.

## 例

暗号化されたエントリを含むアーカイブを作成します。

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry1.bin", new MemoryStream(new byte[] {0x00, 0xFF} ), new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")), new FileInfo("data1.bin")); 
        archive.Save(zipFile);
    }
}
```

### 関連項目

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Func&lt;Stream&gt;, ArchiveEntrySettings) {#createentry}

アーカイブ内に単一のエントリを作成します。

```csharp
public ArchiveEntry CreateEntry(string name, Func<Stream> streamProvider, 
    ArchiveEntrySettings newEntrySettings = null)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| name | String | エントリの名前。 |
| streamProvider | Func`1 | エントリ用の入力ストリームを提供するメソッドです。 |
| newEntrySettings | ArchiveEntrySettings | 追加された [`ArchiveEntry`](../../archiveentry/) アイテムに使用される圧縮および暗号化設定。 |

### 戻り値

Zip エントリ インスタンス。

### 例外

| 例外 | 条件 |
| --- | --- |
| ObjectDisposedException | アーカイブが破棄された場合にスローされます。 |
| ArgumentException | *name* が null または空、あるいは *streamProvider* が null の場合にスローされます。 |
| InvalidOperationException | アーカイブがエントリの追加をサポートしていない場合にスローされます。 |

## 備考

このメソッドは .NET Framework 4.0 以降および .NET Standard 2.0 以降のバージョン向けです。

## 例

暗号化されたエントリを含むアーカイブを作成します。

```csharp
System.Func<Stream> provider = delegate(){ return new MemoryStream(new byte[]{0xFF, 0x00}); };
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry1.bin", provider, new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")))); 
        archive.Save(zipFile);
    }
}
```

### 関連項目

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)


