---
title: "IArchiveFileEntry"
second_title: "Aspose.ZIP for Java API 참조"
description: "이 인터페이스는 아카이브 파일 항목을 나타냅니다."
type: docs
weight: 162
url: /ko/java/com.aspose.zip/iarchivefileentry/
---
```
public interface IArchiveFileEntry
```

이 인터페이스는 아카이브 파일 항목을 나타냅니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | 제공된 스트림으로 항목을 추출합니다. |
| [extract(String path)](#extract-java.lang.String-) | 제공된 경로를 사용하여 파일 시스템에 항목을 추출합니다. |
| [getLength()](#getLength--) | 항목의 길이를 바이트 단위로 가져옵니다. |
| [getName()](#getName--) | 항목의 이름을 가져옵니다. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public abstract void extract(OutputStream destination)
```


제공된 스트림으로 항목을 추출합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 대상 | java.io.OutputStream | 대상 스트림. 쓰기 가능해야 합니다. |

### extract(String path) {#extract-java.lang.String-}
```
public abstract File extract(String path)
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
public abstract Long getLength()
```


항목의 길이를 바이트 단위로 가져옵니다.

**Returns:**
java.lang.Long - 항목의 길이(바이트 단위)
### getName() {#getName--}
```
public abstract String getName()
```


항목의 이름을 가져옵니다.

압축 전용 아카이브, 예를 들어 gzip, bzip2, lzip, lzma, xz, z는 헤더에서 다른 이름을 찾을 수 없으면 "File.bin"이라는 이름을 가집니다.

**Returns:**
java.lang.String - 항목의 이름
