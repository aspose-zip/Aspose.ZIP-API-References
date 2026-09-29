---
title: "TarEntry"
second_title: "Aspose.ZIP for Java API 참조"
description: "tar 아카이브 내 단일 파일을 나타냅니다."
type: docs
weight: 126
url: /ko/java/com.aspose.zip/tarentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class TarEntry implements IArchiveFileEntry
```

tar 아카이브 내 단일 파일을 나타냅니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | 제공된 스트림으로 항목을 추출합니다. |
| [extract(String path)](#extract-java.lang.String-) | 제공된 경로를 사용하여 파일 시스템에 항목을 추출합니다. |
| [getLength()](#getLength--) | 항목의 길이를 바이트 단위로 가져옵니다. |
| [getModificationTime()](#getModificationTime--) | 파일 또는 디렉터리의 수정 시간을 가져옵니다. |
| [getName()](#getName--) | 아카이브 내 항목의 이름을 가져옵니다. |
| [getUncompressedSize()](#getUncompressedSize--) | 원본 파일의 크기를 가져옵니다. |
| [isDirectory()](#isDirectory--) | 항목이 디렉터리를 나타내는지 여부를 나타내는 값을 가져옵니다. |
| [open()](#open--) | 추출을 위해 항목을 열고 항목 내용을 포함하는 스트림을 제공합니다. |
| [setName(String value)](#setName-java.lang.String-) | 아카이브 내 항목의 이름을 설정합니다. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


제공된 스트림으로 항목을 추출합니다.

tar 아카이브의 항목을 추출합니다.

```

``````

try (TarArchive archive = new TarArchive("archive.tar")) {
archive.getEntries().get_Item(0).extract(httpResponseStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | Destination stream. Must be writable. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the entry to the filesystem by the path provided.

```

``````

     try (TarArchive archive = new TarArchive("archive.tar")) {
         archive.getEntries().get_Item(0).extract("data.bin");
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| path | java.lang.String | 대상 파일의 경로입니다. 파일이 이미 존재하면 덮어쓰게 됩니다. |

**Returns:**
java.io.File - 추출된 파일의 파일 정보
### getLength() {#getLength--}
```
public final Long getLength()
```


항목의 길이를 바이트 단위로 가져옵니다.

**Returns:**
java.lang.Long - 항목의 길이(바이트 단위)
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


파일 또는 디렉터리의 수정 시간을 가져옵니다.

**Returns:**
java.util.Date - 파일 또는 디렉터리의 수정 시간입니다.
### getName() {#getName--}
```
public final String getName()
```


아카이브 내 항목의 이름을 가져옵니다.

**Returns:**
java.lang.String - 아카이브 내 항목의 이름
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


원본 파일의 크기를 가져옵니다.

`Length`([getLength](../../com.aspose.zip/tarentry\#getLength--))와 동일한 값을 가집니다.

**Returns:**
long - 원본 파일의 크기입니다.
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


항목이 디렉터리를 나타내는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 항목이 디렉터리를 나타내는지 여부를 나타내는 값
### open() {#open--}
```
public final InputStream open()
```


추출을 위해 항목을 열고 항목 내용을 포함하는 스트림을 제공합니다.


사용법:

```

``````

InputStream decompressed = entry.open();
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
fileStream.write(buffer, 0, bytesRead);
}
 
```

Read from the stream to get the original content of the file. See examples section.

**Returns:**
java.io.InputStream - the stream that represents the contents of the entry
### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Sets the name of the entry within the archive.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the name of the entry within the archive |

