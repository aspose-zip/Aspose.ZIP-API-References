---
title: "CabEntry"
second_title: "Aspose.ZIP for Java API 참조"
description: "CAB 아카이브 내의 단일 파일을 나타냅니다."
type: docs
weight: 46
url: /ko/java/com.aspose.zip/cabentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public final class CabEntry implements IArchiveFileEntry
```

CAB 아카이브 내의 단일 파일을 나타냅니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | 제공된 스트림으로 항목을 추출합니다. |
| [extract(String path)](#extract-java.lang.String-) | 제공된 경로를 사용하여 파일 시스템에 항목을 추출합니다. |
| [getLength()](#getLength--) | 항목의 길이를 바이트 단위로 가져옵니다. |
| [getModificationTime()](#getModificationTime--) | 마지막 수정 날짜와 시간을 가져옵니다. |
| [getName()](#getName--) | 아카이브 내 항목의 이름을 가져옵니다. |
| [open()](#open--) | 추출을 위해 항목을 열고 항목 내용을 포함하는 스트림을 제공합니다. |
| [toString()](#toString--) | [CabEntry](../../com.aspose.zip/cabentry) 클래스 인스턴스의 문자열 표현을 반환합니다. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


제공된 스트림으로 항목을 추출합니다.

CAB 아카이브의 항목을 추출합니다.

```

``````

try (CabArchive archive = new CabArchive("archive.cab")) {
archive.getEntries().get(0).extract(httpResponseStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream. Must be writable |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the entry to the filesystem by the path provided.

```

``````

     try (CabArchive archive = new CabArchive("archive.cab")) {
         archive.getEntries().get(0).extract("data.bin");
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| path | java.lang.String | 대상 파일의 경로입니다. 파일이 이미 존재하면 덮어쓰게 됩니다. |

**Returns:**
java.io.File - 구성된 파일의 파일 정보
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


마지막 수정 날짜와 시간을 가져옵니다.

**Returns:**
java.util.Date - 마지막 수정 날짜 및 시간.
### getName() {#getName--}
```
public final String getName()
```


아카이브 내 항목의 이름을 가져옵니다.

**Returns:**
java.lang.String - 아카이브 내 항목의 이름
### open() {#open--}
```
public final InputStream open()
```


추출을 위해 항목을 열고 항목 내용을 포함하는 스트림을 제공합니다.

사용법:

```

``````

CabArchive archive = new CabArchive("archive.cab");
CabEntry entry = archive.getEntries().get(0);
try (FileOutputStream fileStream = new FileOutputStream("data.bin")) {
try (InputStream decompressed = entry.open()) {
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
fileStream.write(buffer, 0, bytesRead);
}
}
} catch (IOException ex) {
}
 
```

Read from the stream to get the original content of a file. See examples section.

**Returns:**
java.io.InputStream - the stream that represents the contents of the entry
### toString() {#toString--}
```
public String toString()
```


Returns string representation of the instance of the [CabEntry](../../com.aspose.zip/cabentry) class.

**Returns:**
java.lang.String - string representation of this object
