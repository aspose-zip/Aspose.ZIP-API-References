---
title: "ArchiveFactory"
second_title: "Aspose.ZIP for Java API 참조"
description: "아카이브 형식을 감지하고 아카이브 유형에 따라 적절한 객체를 생성합니다."
type: docs
weight: 31
url: /ko/java/com.aspose.zip/archivefactory/
---

**Inheritance:**
java.lang.Object
```
public final class ArchiveFactory
```

아카이브 형식을 감지하고 아카이브 유형에 따라 적절한 [IArchive](../../com.aspose.zip/iarchive) 객체를 생성합니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [compressDirectory(String path, String outputFileName, ArchiveFormat archiveFormat)](#compressDirectory-java.lang.String-java.lang.String-com.aspose.zip.ArchiveFormat-) | 지정된 디렉터리를 제공된 아카이브 형식을 사용하여 아카이브 파일로 압축합니다. |
| [getArchive(InputStream stream)](#getArchive-java.io.InputStream-) | 주어진 스트림에 의해 지정된 아카이브 유형에 따라 아카이브 형식을 감지하고 적절한 [IArchive](../../com.aspose.zip/iarchive) 객체를 생성합니다. |
| [getArchive(InputStream stream, String password)](#getArchive-java.io.InputStream-java.lang.String-) | 주어진 스트림에 의해 지정된 암호화된 아카이브 유형에 따라 아카이브 형식을 감지하고 적절한 [IArchive](../../com.aspose.zip/iarchive) 객체를 생성합니다. |
| [getArchive(String path)](#getArchive-java.lang.String-) | 주어진 경로에 의해 지정된 아카이브 유형에 따라 아카이브 형식을 감지하고 적절한 [IArchive](../../com.aspose.zip/iarchive) 객체를 생성합니다. |
### compressDirectory(String path, String outputFileName, ArchiveFormat archiveFormat) {#compressDirectory-java.lang.String-java.lang.String-com.aspose.zip.ArchiveFormat-}
```
public static void compressDirectory(String path, String outputFileName, ArchiveFormat archiveFormat)
```


지정된 디렉터리를 제공된 아카이브 형식을 사용하여 아카이브 파일로 압축합니다.

CompressDirectory 메서드를 사용하는 예시는 다음과 같습니다:

```

``````

String directoryPath = "C:\\path\\to\\your\\directory";
ArchiveFormat format = ArchiveFormat.Zip;
ArchiveFactory.compressDirectory(directoryPath, "result", format);
// 지정된 경로에 있는 디렉터리의 내용을 포함한 ZIP 파일을 생성합니다.
 
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
