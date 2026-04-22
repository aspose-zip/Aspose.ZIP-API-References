---
title: Archive.CreateEntry
second_title: Aspose.ZIP for .NET API リファレンス
description: Archive 方法. アーカイブ内に単一のエントリを作成します
type: docs
weight: 50
url: /ja/net/aspose.zip/archive/createentry/
---
## CreateEntry(string, string, bool, ArchiveEntrySettings) {#createentry_3}

アーカイブ内に単一のエントリを作成します。

```csharp
public ArchiveEntry CreateEntry(string name, string path, bool openImmediately = false, 
    ArchiveEntrySettings newEntrySettings = null)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| name | String | エントリの名前。 |
| path | String | 新しいファイルの完全修飾名、または圧縮する相対ファイル名。 |
| openImmediately | Boolean | ファイルをすぐに開く場合は true、それ以外の場合はアーカイブ保存時にファイルを開きます。 |
| newEntrySettings | ArchiveEntrySettings | 追加に使用される圧縮と暗号化の設定[`ArchiveEntry`](../../archiveentry/)アイテム。 |

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
* 名前空間 [Aspose.Zip](../../archive/)
* 組み立て [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, ArchiveEntrySettings) {#createentry_1}

アーカイブ内に単一のエントリを作成します。

```csharp
public ArchiveEntry CreateEntry(string name, Stream source, 
    ArchiveEntrySettings newEntrySettings = null)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| name | String | エントリの名前。 |
| source | Stream | エントリの入力ストリーム。 |
| newEntrySettings | ArchiveEntrySettings | 追加に使用される圧縮と暗号化の設定[`ArchiveEntry`](../../archiveentry/)アイテム。 |

### 戻り値

zip エントリのインスタンス。

### 例

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
* 名前空間 [Aspose.Zip](../../archive/)
* 組み立て [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool, ArchiveEntrySettings) {#createentry}

アーカイブ内に単一のエントリを作成します。

```csharp
public ArchiveEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false, 
    ArchiveEntrySettings newEntrySettings = null)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| name | String | エントリの名前。 |
| fileInfo | FileInfo | 圧縮するファイルのメタデータ。 |
| openImmediately | Boolean | ファイルをすぐに開く場合は true、それ以外の場合はアーカイブ保存時にファイルを開きます。 |
| newEntrySettings | ArchiveEntrySettings | 追加に使用される圧縮と暗号化の設定[`ArchiveEntry`](../../archiveentry/)アイテム。 |

### 戻り値

zip エントリのインスタンス。

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

それぞれ異なる暗号化方法とパスワードで暗号化されたエントリでアーカイブを作成します。

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
* 名前空間 [Aspose.Zip](../../archive/)
* 組み立て [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, ArchiveEntrySettings, FileSystemInfo) {#createentry_2}

アーカイブ内に単一のエントリを作成します。

```csharp
public ArchiveEntry CreateEntry(string name, Stream source, ArchiveEntrySettings newEntrySettings, 
    FileSystemInfo fileInfo)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| name | String | エントリの名前。 |
| source | Stream | エントリの入力ストリーム。 |
| newEntrySettings | ArchiveEntrySettings | 追加に使用される圧縮と暗号化の設定[`ArchiveEntry`](../../archiveentry/)アイテム。 |
| fileInfo | FileSystemInfo | 圧縮するファイルまたはフォルダーのメタデータ。 |

### 戻り値

zip エントリのインスタンス。

### 例外

| 例外 | 調子 |
| --- | --- |
| InvalidOperationException | 両方*source*と*fileInfo*null または*source*はヌルであり、*fileInfo*ディレクトリの略です。 |

### 備考

エントリ名は、*name*パラメータ。で提供されているファイル名*fileInfo*パラメータは、エントリ名には影響しません。

*fileInfo*参照できますDirectoryInfoエントリがディレクトリの場合。

### 例

暗号化されたエントリでアーカイブを作成します。

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
* 名前空間 [Aspose.Zip](../../archive/)
* 組み立て [Aspose.Zip](../../../)


