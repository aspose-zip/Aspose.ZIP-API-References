---
title: "AlzEntry"
second_title: "Aspose.ZIP for Java API 참조"
description: "ALZ 아카이브 내 파일 항목과 해당 메타데이터를 나타냅니다."
type: docs
weight: 13
url: /ko/java/com.aspose.zip/alzentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class AlzEntry implements IArchiveFileEntry
```

ALZ 아카이브 내 파일 항목과 해당 메타데이터를 나타냅니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | 엔트리를 쓰기 가능한 스트림으로 추출합니다. |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | 옵션 비밀번호를 사용하여 엔트리를 쓰기 가능한 스트림으로 추출합니다. |
| [extract(String path)](#extract-java.lang.String-) | 엔트리를 지정된 파일로 추출합니다. |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | 옵션 비밀번호를 사용하여 엔트리를 지정된 파일로 추출합니다. |
| [getCompressedSize()](#getCompressedSize--) | 엔트리 데이터의 압축된 크기를 바이트 단위로 가져옵니다. |
| [getLength()](#getLength--) | 이 엔트리의 압축 해제된 길이를 가져옵니다. |
| [getName()](#getName--) | 아카이브에 저장된 엔트리 이름을 가져옵니다. |
| [getUncompressedSize()](#getUncompressedSize--) | 엔트리 데이터의 압축 해제된 크기를 바이트 단위로 가져옵니다. |
| [isDirectory()](#isDirectory--) | 이 엔트리가 디렉터리를 나타내는지 여부를 가져옵니다. |
| [open()](#open--) | 엔트리를 열고 압축 해제된 데이터를 포함하는 스트림을 제공합니다. |
| [open(String password)](#open-java.lang.String-) | 엔트리를 열고 압축 해제된 데이터를 포함하는 스트림을 제공합니다. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


엔트리를 쓰기 가능한 스트림으로 추출합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 대상 | java.io.OutputStream | 대상 스트림 |

### extract(OutputStream destination, String password) {#extract-java.io.OutputStream-java.lang.String-}
```
public final void extract(OutputStream destination, String password)
```


옵션 비밀번호를 사용하여 엔트리를 쓰기 가능한 스트림으로 추출합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 대상 | java.io.OutputStream | 대상 스트림 |
| password | java.lang.String | 이 엔트리의 옵션 비밀번호 |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


엔트리를 지정된 파일로 추출합니다. 기존 파일이 덮어쓰기됩니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| path | java.lang.String | 대상 파일 경로 |

**Returns:**
java.io.File - 추출된 파일
### extract(String path, String password) {#extract-java.lang.String-java.lang.String-}
```
public final File extract(String path, String password)
```


옵션 비밀번호를 사용하여 엔트리를 지정된 파일로 추출합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| path | java.lang.String | 대상 파일 경로 |
| password | java.lang.String | 이 엔트리의 옵션 비밀번호 |

**Returns:**
java.io.File - 추출된 파일
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


엔트리 데이터의 압축된 크기를 바이트 단위로 가져옵니다.

**Returns:**
long - 압축된 크기(바이트 단위)
### getLength() {#getLength--}
```
public final Long getLength()
```


이 엔트리의 압축 해제된 길이를 가져옵니다.

**Returns:**
java.lang.Long - 압축 해제된 길이(바이트 단위)
### getName() {#getName--}
```
public final String getName()
```


아카이브에 저장된 엔트리 이름을 가져옵니다.

**Returns:**
java.lang.String - 항목 이름
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


엔트리 데이터의 압축 해제된 크기를 바이트 단위로 가져옵니다.

**Returns:**
long - 압축 해제된 크기(바이트 단위)
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


이 엔트리가 디렉터리를 나타내는지 여부를 가져옵니다.

**Returns:**
boolean - 디렉터리 항목에 대해 `true`
### open() {#open--}
```
public final InputStream open()
```


엔트리를 열고 압축 해제된 데이터를 포함하는 스트림을 제공합니다.

**Returns:**
java.io.InputStream - 압축 해제된 항목 데이터를 포함하는 스트림
### open(String password) {#open-java.lang.String-}
```
public final InputStream open(String password)
```


엔트리를 열고 압축 해제된 데이터를 포함하는 스트림을 제공합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| password | java.lang.String | 이 엔트리의 옵션 비밀번호 |

**Returns:**
java.io.InputStream - 압축 해제된 항목 데이터를 포함하는 스트림
