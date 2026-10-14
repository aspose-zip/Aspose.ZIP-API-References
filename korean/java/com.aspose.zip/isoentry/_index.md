---
title: "IsoEntry"
second_title: "Aspose.ZIP for Java API 참조"
description: "ISO 아카이브 내의 파일 또는 디렉터리 항목을 나타냅니다."
type: docs
weight: 72
url: /ko/java/com.aspose.zip/isoentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class IsoEntry implements IArchiveFileEntry
```

ISO 아카이브 내의 항목(파일 또는 디렉터리)을 나타냅니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | 제공된 스트림으로 항목을 추출합니다. |
| [extract(String path)](#extract-java.lang.String-) | 제공된 경로를 사용하여 파일 시스템에 항목을 추출합니다. |
| [getLength()](#getLength--) | 항목의 길이를 가져옵니다. |
| [getModificationTime()](#getModificationTime--) | 마지막 수정 날짜와 시간을 가져옵니다. |
| [getName()](#getName--) | 항목의 이름을 가져옵니다. |
| [isDirectory()](#isDirectory--) | 항목이 디렉터리인지 여부를 나타내는 값을 가져옵니다. |
| [toString()](#toString--) | 현재 항목을 나타내는 문자열을 반환합니다. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public void extract(OutputStream destination)
```


제공된 스트림으로 항목을 추출합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 대상 | java.io.OutputStream | 대상 스트림 |

### extract(String path) {#extract-java.lang.String-}
```
public File extract(String path)
```


제공된 경로를 사용하여 파일 시스템에 항목을 추출합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| path | java.lang.String | 대상 파일의 경로입니다. 파일이 이미 존재하면 덮어쓰게 됩니다. |

**Returns:**
java.io.File - 추출된 데이터를 포함하는 java.io.File 인스턴스
### getLength() {#getLength--}
```
public Long getLength()
```


항목의 길이를 가져옵니다.

**Returns:**
java.lang.Long - 항목의 길이
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


마지막 수정 날짜와 시간을 가져옵니다.

**Returns:**
java.util.Date - 마지막 수정 날짜 및 시간
### getName() {#getName--}
```
public final String getName()
```


항목의 이름을 가져옵니다.

**Returns:**
java.lang.String - 항목의 이름
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


항목이 디렉터리인지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 항목이 디렉터리를 나타내는지 여부를 나타내는 값
### toString() {#toString--}
```
public String toString()
```


현재 항목을 나타내는 문자열을 반환합니다.

**Returns:**
java.lang.String - 항목의 이름
