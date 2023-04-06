---
title: TarArchive.CreateEntry
second_title: Aspose.ZIP for .NET API リファレンス
description: TarArchive 方法. アーカイブ内に単一のエントリを作成します
type: docs
weight: 80
url: /ja/net/aspose.zip.tar/tararchive/createentry/
---
## CreateEntry(string, Stream, FileSystemInfo) {#createentry_1}

アーカイブ内に単一のエントリを作成します。

```csharp
public TarEntry CreateEntry(string name, Stream source, FileSystemInfo fileInfo = null)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| name | String | エントリの名前。 |
| source | Stream | エントリの入力ストリーム。 |
| fileInfo | FileSystemInfo | 圧縮するファイルまたはフォルダーのメタデータ。 |

### 戻り値

tar エントリ インスタンス。

### 例外

| 例外 | 調子 |
| --- | --- |
| PathTooLongException | *name* IEEE 1003.1-1998 標準の tar には長すぎます。 |
| ArgumentException | 一部としてのファイル名*name*、100 シンボルを超えています。 |

### 備考

エントリ名は、*name*パラメータ。で提供されているファイル名*fileInfo*パラメータは、エントリ名には影響しません。

*fileInfo*参照できますDirectoryInfoエントリがディレクトリの場合。

### 例

```csharp
using (var archive = new TarArchive())
{
   archive.CreateEntry("bytes", new MemoryStream(new byte[] {0x00, 0xFF}));
   archive.Save(tarFile);
}
```

### 関連項目

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* 名前空間 [Aspose.Zip.Tar](../../tararchive/)
* 組み立て [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool) {#createentry}

アーカイブ内に単一のエントリを作成します。

```csharp
public TarEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| name | String | エントリの名前。 |
| fileInfo | FileInfo | 圧縮するファイルまたはフォルダーのメタデータ。 |
| openImmediately | Boolean | ファイルをすぐに開く場合は true、それ以外の場合はアーカイブ保存時にファイルを開きます。 |

### 戻り値

tar エントリ インスタンス。

### 例外

| 例外 | 調子 |
| --- | --- |
| PathTooLongException | *name* IEEE 1003.1-1998 標準の tar には長すぎます。 |
| ArgumentException | 一部としてのファイル名*name*、100 シンボルを超えています。 |

### 備考

エントリ名は、*name*パラメータ。で提供されているファイル名*fileInfo*パラメータは、エントリ名には影響しません。

*fileInfo*参照できますDirectoryInfoエントリがディレクトリの場合。

ファイルがすぐに開かれた場合*openImmediately*パラメータは、アーカイブが破棄されるまでブロックされます。

### 例

```csharp
FileInfo fi = new FileInfo("data.bin");
using (var archive = new TarArchive())
{
   archive.CreateEntry("data.bin", fi);
   archive.Save(tarFile);
}
```

### 関連項目

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* 名前空間 [Aspose.Zip.Tar](../../tararchive/)
* 組み立て [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool) {#createentry_2}

アーカイブ内に単一のエントリを作成します。

```csharp
public TarEntry CreateEntry(string name, string path, bool openImmediately = false)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| name | String | エントリの名前。 |
| path | String | 圧縮するファイルへのパス。 |
| openImmediately | Boolean | ファイルをすぐに開く場合は true、それ以外の場合はアーカイブ保存時にファイルを開きます。 |

### 戻り値

tar エントリ インスタンス。

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentNullException | *path*無効である。 |
| SecurityException | 呼び出し元には、アクセスに必要なアクセス許可がありません。 |
| ArgumentException | の*path*が空であるか、空白のみが含まれているか、無効な文字が含まれています。 - または - の一部としてのファイル名*name*、100 シンボルを超えています。 |
| UnauthorizedAccessException | ファイルへのアクセス*path*否定された。 |
| PathTooLongException | 指定された*path*、ファイル名、またはその両方がシステム定義の最大長を超えています。たとえば、Windows ベースのプラットフォームでは、パスは 248 文字未満、ファイル名は 260 文字未満である必要があります。 - また -*name* IEEE 1003.1-1998 標準の tar には長すぎます。 |
| NotSupportedException | ファイル*path*文字列の途中にコロン (:) が含まれています。 |

### 備考

エントリ名は、*name*パラメータ。で提供されているファイル名*path*パラメータは、エントリ名には影響しません。

ファイルがすぐに開かれた場合*openImmediately*パラメータは、アーカイブが破棄されるまでブロックされます。

### 例

```csharp
using (var archive = new TarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save(outputTarFile);
}
```

### 関連項目

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* 名前空間 [Aspose.Zip.Tar](../../tararchive/)
* 組み立て [Aspose.Zip](../../../)


