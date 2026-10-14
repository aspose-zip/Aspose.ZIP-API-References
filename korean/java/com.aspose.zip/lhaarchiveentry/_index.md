---
title: "LhaArchiveEntry"
second_title: "Aspose.ZIP for Java API 참조"
description: "Lha 아카이브 내의 단일 파일을 나타냅니다."
type: docs
weight: 76
url: /ko/java/com.aspose.zip/lhaarchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class LhaArchiveEntry implements IArchiveFileEntry
```

Lha 아카이브 내의 단일 파일을 나타냅니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [extract(File file)](#extract-java.io.File-) | Lha 아카이브 항목을 파일로 추출합니다. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | 제공된 스트림으로 항목을 추출합니다. |
| [extract(String path)](#extract-java.lang.String-) | Lha 아카이브 항목을 경로를 통해 파일 시스템에 추출합니다. |
| [getLastModified()](#getLastModified--) | 항목의 마지막 수정 시간을 가져옵니다. |
| [getLength()](#getLength--) | 항목의 길이를 바이트 단위로 가져옵니다. |
| [getModificationTime()](#getModificationTime--) | 항목의 마지막 수정 시간을 가져옵니다. |
| [getName()](#getName--) | 항목의 이름을 가져옵니다. |
| [getPath()](#getPath--) | 항목의 전체 경로를 가져옵니다. |
| [isDirectory()](#isDirectory--) | 이 항목이 디렉터리인지 여부를 나타내는 값을 가져옵니다. |
### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Lha 아카이브 항목을 파일로 추출합니다.

```

``````

try (FileInputStream lhaFile = new FileInputStream("archive.lha")) {
try (LhaArchive archive = new LhaArchive(lhaFile)) {
archive.getEntries().get(0).extract(new File("extracted.bin"));
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | File for storing decompressed data.

Does nothing for directory entry |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts the entry to the stream provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts Lha archive entry to a filesystem by path.

```

``````

     try (FileInputStream lhaFile = new FileInputStream("archive.lha")) {
         try (LhaArchive archive = new LhaArchive(lhaFile)) {
             archive.getEntries().get(0).extract("extracted.bin");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| path | java.lang.String | 압축 해제된 데이터를 저장할 파일의 경로 |

**Returns:**
java.io.File - 추출된 데이터를 포함하는 java.io.File 인스턴스
### getLastModified() {#getLastModified--}
```
public final Date getLastModified()
```


항목의 마지막 수정 시간을 가져옵니다.

**Returns:**
java.util.Date - 항목의 마지막 수정 시간
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


항목의 마지막 수정 시간을 가져옵니다.

**Returns:**
java.util.Date - 항목의 마지막 수정 시간
### getName() {#getName--}
```
public final String getName()
```


항목의 이름을 가져옵니다.

압축 전용 아카이브, 예를 들어 gzip, bzip2, lzip, lzma, xz, z는 헤더에서 다른 이름을 찾을 수 없으면 "File.bin"이라는 이름을 가집니다.

**Returns:**
java.lang.String - 항목의 이름
### getPath() {#getPath--}
```
public final String getPath()
```


항목의 전체 경로를 가져옵니다.

**Returns:**
java.lang.String - 항목의 전체 경로
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


이 항목이 디렉터리인지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 이 항목이 디렉터리인지 여부를 나타내는 값.
