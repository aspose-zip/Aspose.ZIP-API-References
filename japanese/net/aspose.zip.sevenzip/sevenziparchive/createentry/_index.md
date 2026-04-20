---
title: SevenZipArchive.CreateEntry
second_title: Aspose.ZIP for .NET API リファレンス
description: SevenZipArchive 方法. アーカイブ内に単一のエントリを作成します
type: docs
weight: 50
url: /ja/net/aspose.zip.sevenzip/sevenziparchive/createentry/
---
## CreateEntry(string, FileInfo, bool, SevenZipEntrySettings) {#createentry}

アーカイブ内に単一のエントリを作成します。

```csharp
public SevenZipArchiveEntry CreateEntry(string name, FileInfo fileInfo, 
    bool openImmediately = false, SevenZipEntrySettings newEntrySettings = null)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| name | String | エントリの名前。 |
| fileInfo | FileInfo | 圧縮するファイルのメタデータ。 |
| openImmediately | Boolean | ファイルをすぐに開く場合は true、それ以外の場合はアーカイブ保存時にファイルを開きます。 |
| newEntrySettings | SevenZipEntrySettings | 追加に使用される圧縮と暗号化の設定[`SevenZipArchiveEntry`](../../sevenziparchiveentry/)アイテム。 |

### 戻り値

7 つの Zip エントリ インスタンス。

### 例外

| 例外 | 調子 |
| --- | --- |
| UnauthorizedAccessException | *fileInfo*読み取り専用またはディレクトリです。 |
| DirectoryNotFoundException | 指定されたパスは、マップされていないドライブ上にあるなど、無効です。 |
| IOException | ファイルは既に開いています。 |

### 備考

エントリ名は、*name*パラメータ。で提供されているファイル名*fileInfo*パラメータは、エントリ名には影響しません。

ファイルがすぐに開かれた場合*openImmediately*パラメータは、アーカイブが保存されるまでブロックされます。

### 例

それぞれ異なるパスワードで暗号化されたエントリでアーカイブを作成します。

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
* 名前空間 [Aspose.Zip.SevenZip](../../sevenziparchive/)
* 組み立て [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, SevenZipEntrySettings, FileSystemInfo) {#createentry_2}

アーカイブ内に単一のエントリを作成します。

```csharp
public SevenZipArchiveEntry CreateEntry(string name, Stream source, 
    SevenZipEntrySettings newEntrySettings, FileSystemInfo fileInfo)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| name | String | エントリの名前。 |
| source | Stream | エントリの入力ストリーム。 |
| newEntrySettings | SevenZipEntrySettings | 追加に使用される圧縮と暗号化の設定[`SevenZipArchiveEntry`](../../sevenziparchiveentry/)アイテム。 |
| fileInfo | FileSystemInfo | 圧縮するファイルまたはフォルダーのメタデータ。 |

### 戻り値

SevenZip エントリ インスタンス。

### 例外

| 例外 | 調子 |
| --- | --- |
| InvalidOperationException | 両方*source*と*fileInfo*null または*source*はヌルであり、*fileInfo*ディレクトリの略です。 |

### 備考

エントリ名は、*name*パラメータ。で提供されているファイル名*fileInfo*パラメータは、エントリ名には影響しません。

*fileInfo*参照できますDirectoryInfoエントリがディレクトリの場合。

### 例

LZMA2 で圧縮された暗号化エントリでアーカイブを作成します。

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
* 名前空間 [Aspose.Zip.SevenZip](../../sevenziparchive/)
* 組み立て [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, SevenZipEntrySettings) {#createentry_1}

アーカイブ内に単一のエントリを作成します。

```csharp
public SevenZipArchiveEntry CreateEntry(string name, Stream source, 
    SevenZipEntrySettings newEntrySettings = null)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| name | String | エントリの名前。 |
| source | Stream | エントリの入力ストリーム。 |
| newEntrySettings | SevenZipEntrySettings | 追加に使用される圧縮と暗号化の設定[`SevenZipArchiveEntry`](../../sevenziparchiveentry/)アイテム。 |

### 戻り値

zip エントリのインスタンス。

### 例

LZMA2 圧縮とすべてのエントリの暗号化を使用して 7z アーカイブを作成します。

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
* 名前空間 [Aspose.Zip.SevenZip](../../sevenziparchive/)
* 組み立て [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool, SevenZipEntrySettings) {#createentry_3}

アーカイブ内に単一のエントリを作成します。

```csharp
public SevenZipArchiveEntry CreateEntry(string name, string path, bool openImmediately = false, 
    SevenZipEntrySettings newEntrySettings = null)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| name | String | エントリの名前。 |
| path | String | 新しいファイルの完全修飾名、または圧縮する相対ファイル名。 |
| openImmediately | Boolean | ファイルをすぐに開く場合は true、それ以外の場合はアーカイブ保存時にファイルを開きます。 |
| newEntrySettings | SevenZipEntrySettings | 追加に使用される圧縮と暗号化の設定[`SevenZipArchiveEntry`](../../sevenziparchiveentry/)アイテム。 |

### 戻り値

zip エントリのインスタンス。

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentNullException | *path*無効である。 |
| SecurityException | 呼び出し元には、アクセスに必要なアクセス許可がありません。 |
| ArgumentException | の*path*が空であるか、空白のみが含まれているか、無効な文字が含まれています。 |
| UnauthorizedAccessException | ファイルへのアクセス*path*否定された。 |
| PathTooLongException | 指定された*path*、ファイル名、またはその両方がシステム定義の最大長を超えています。たとえば、Windows ベースのプラットフォームでは、パスは 248 文字未満、ファイル名は 260 文字未満である必要があります。 |
| NotSupportedException | ファイル*path*文字列の途中にコロン (:) が含まれています。 |

### 備考

エントリ名は、*name*パラメータ。で提供されているファイル名*path*パラメータは、エントリ名には影響しません。

ファイルがすぐに開かれた場合*openImmediately*パラメータは、アーカイブが保存されるまでブロックされます。

### 例

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
* 名前空間 [Aspose.Zip.SevenZip](../../sevenziparchive/)
* 組み立て [Aspose.Zip](../../../)


