---
title: "ArchiveFactory"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "アーカイブ形式を検出し、アーカイブの種類に応じて適切なオブジェクトを作成します。"
type: docs
weight: 31
url: /ja/java/com.aspose.zip/archivefactory/
---

**Inheritance:**
java.lang.Object
```
public final class ArchiveFactory
```

アーカイブ形式を検出し、アーカイブの種類に応じて適切な [IArchive](../../com.aspose.zip/iarchive) オブジェクトを作成します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [compressDirectory(String path, String outputFileName, ArchiveFormat archiveFormat)](#compressDirectory-java.lang.String-java.lang.String-com.aspose.zip.ArchiveFormat-) | 指定されたディレクトリを、提供されたアーカイブ形式を使用してアーカイブファイルに圧縮します。 |
| [getArchive(InputStream stream)](#getArchive-java.io.InputStream-) | 指定されたストリームで指定されたアーカイブの種類に応じて、アーカイブ形式を検出し、適切な [IArchive](../../com.aspose.zip/iarchive) オブジェクトを作成します。 |
| [getArchive(InputStream stream, String password)](#getArchive-java.io.InputStream-java.lang.String-) | 指定されたストリームで指定された暗号化アーカイブの種類に応じて、アーカイブ形式を検出し、適切な [IArchive](../../com.aspose.zip/iarchive) オブジェクトを作成します。 |
| [getArchive(String path)](#getArchive-java.lang.String-) | 指定されたパスで指定されたアーカイブの種類に応じて、アーカイブ形式を検出し、適切な [IArchive](../../com.aspose.zip/iarchive) オブジェクトを作成します。 |
### compressDirectory(String path, String outputFileName, ArchiveFormat archiveFormat) {#compressDirectory-java.lang.String-java.lang.String-com.aspose.zip.ArchiveFormat-}
```
public static void compressDirectory(String path, String outputFileName, ArchiveFormat archiveFormat)
```


指定されたディレクトリを、提供されたアーカイブ形式を使用してアーカイブファイルに圧縮します。

以下は CompressDirectory メソッドの使用例です：

```

``````

String directoryPath = "C:\\path\\to\\your\\directory";
ArchiveFormat format = ArchiveFormat.Zip;
ArchiveFactory.compressDirectory(directoryPath, "result", format);
// これにより、指定されたパスのディレクトリの内容を含む ZIP ファイルが作成されます。
 
```

This method will create an archive file at the location specified by the `path` parameter. The name of the archive file will typically be the directory name followed by the appropriate file extension based on the `archiveFormat`. The directory itself is not modified or deleted.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the directory that will be compressed |
| outputFileName | java.lang.String | destination file name |
| archiveFormat | [ArchiveFormat](../../com.aspose.zip/archiveformat) | the format of the archive to create (e.g., zip, rar, tar, etc.) |

### getArchive(InputStream stream) {#getArchive-java.io.InputStream-}
```
public static IArchive getArchive(InputStream stream)
```


Detects the archive format and creates the appropriate [IArchive](../../com.aspose.zip/iarchive) object according to the type of archive specified by the given stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | the stream containing the archive data |

**Returns:**
[IArchive](../../com.aspose.zip/iarchive) - an [IArchive](../../com.aspose.zip/iarchive) object representing the archive
### getArchive(InputStream stream, String password) {#getArchive-java.io.InputStream-java.lang.String-}
```
public static IArchive getArchive(InputStream stream, String password)
```


Detects the archive format and creates the appropriate [IArchive](../../com.aspose.zip/iarchive) object according to the type of encrypted archive specified by the given stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | the stream containing the archive data |
| password | java.lang.String | password to decrypt an encrypted archive |

**Returns:**
[IArchive](../../com.aspose.zip/iarchive) - an [IArchive](../../com.aspose.zip/iarchive) object representing the archive
### getArchive(String path) {#getArchive-java.lang.String-}
```
public static IArchive getArchive(String path)
```


Detects the archive format and creates the appropriate [IArchive](../../com.aspose.zip/iarchive) object according to the type of archive specified by the given path.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive to be analyzed |

**Returns:**
[IArchive](../../com.aspose.zip/iarchive) - an [IArchive](../../com.aspose.zip/iarchive) object representing the archive
