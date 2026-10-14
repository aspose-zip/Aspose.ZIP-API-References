---
title: "ArjEntryPlain"
second_title: "Aspose.ZIP for Java API 참조"
description: "ARJ 아카이브 내의 단일 파일을 나타냅니다."
type: docs
weight: 38
url: /ko/java/com.aspose.zip/arjentryplain/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class ArjEntryPlain implements IArchiveFileEntry
```

ARJ 아카이브 내의 단일 파일을 나타냅니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [extract(File file)](#extract-java.io.File-) | ARJ 아카이브 항목을 파일로 추출합니다. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | 제공된 스트림으로 항목을 추출합니다. |
| [extract(String path)](#extract-java.lang.String-) | 제공된 경로를 사용하여 파일 시스템에 항목을 추출합니다. |
| [getCompressedSize()](#getCompressedSize--) | 압축된 파일의 크기를 가져옵니다. |
| [getLength()](#getLength--) | 항목의 길이를 바이트 단위로 가져옵니다. |
| [getName()](#getName--) | 아카이브 내 항목의 이름을 가져옵니다. |
| [getUncompressedSize()](#getUncompressedSize--) | 원본 파일의 크기를 가져옵니다. |
### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


ARJ 아카이브 항목을 파일로 추출합니다.

```

``````

try (FileInputStream arjFile = new FileInputStream("sourceFileName")) {
try (ArjArchive archive = new ArjArchive(arjFile)) {
archive.getEntries().get(0).extract(new File("extracted.bin"));
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | java.io.File for storing decompressed data |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts the entry to the stream provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | Destination stream. Must be writable. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the entry to the filesystem by the path provided.

Extract two entries of rar archive.

```

``````

     try (FileInputStream arjFile = new FileInputStream("archive.arj")) {
         try (ArjArchive archive = new ArjArchive(arjFile)) {
             archive.getEntries().get(0).extract("first.bin");
             archive.getEntries().get(1).extract("second.bin");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| path | java.lang.String | 대상 파일의 경로입니다. 파일이 이미 존재하면 덮어쓰게 됩니다. |

**Returns:**
java.io.File - 구성된 파일의 파일 정보
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


압축된 파일의 크기를 가져옵니다.

**Returns:**
long - 압축된 파일의 크기
### getLength() {#getLength--}
```
public final Long getLength()
```


항목의 길이를 바이트 단위로 가져옵니다.

**Returns:**
java.lang.Long - 항목의 길이(바이트 단위)
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

**Returns:**
long - 원본 파일의 크기
