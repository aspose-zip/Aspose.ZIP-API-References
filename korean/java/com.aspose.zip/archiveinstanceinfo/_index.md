---
title: "ArchiveInstanceInfo"
second_title: "Aspose.ZIP for Java API 참조"
description: "아카이브 인스턴스에 대한 정보를 나타냅니다."
type: docs
weight: 34
url: /ko/java/com.aspose.zip/archiveinstanceinfo/
---

**Inheritance:**
java.lang.Object
```
public final class ArchiveInstanceInfo
```

아카이브 인스턴스에 대한 정보를 나타냅니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [areFileNamesEncrypted()](#areFileNamesEncrypted--) | 아카이브의 엔트리(파일) 이름이 암호화되었는지 여부를 나타내는 값을 가져옵니다. |
| [getArchiveFormatInfo(InputStream stream)](#getArchiveFormatInfo-java.io.InputStream-) | 아카이브 형식 정보를 가져옵니다. |
| [getArchiveFormatInfo(String fileName)](#getArchiveFormatInfo-java.lang.String-) | 아카이브 형식 정보를 가져옵니다. |
| [getArchiveInstanceInfo(InputStream stream)](#getArchiveInstanceInfo-java.io.InputStream-) | 아카이브 인스턴스 정보를 가져옵니다. |
| [getArchiveInstanceInfo(String fileName)](#getArchiveInstanceInfo-java.lang.String-) | 아카이브 인스턴스 정보를 가져옵니다. |
| [getFormatInfo()](#getFormatInfo--) | 아카이브 형식 정보를 가져옵니다. |
| [isContentEncrypted()](#isContentEncrypted--) | 아카이브 내용이 암호화되었는지 여부를 나타내는 값을 가져옵니다. |
### areFileNamesEncrypted() {#areFileNamesEncrypted--}
```
public final boolean areFileNamesEncrypted()
```


아카이브의 엔트리(파일) 이름이 암호화되었는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 아카이브 항목(파일)의 이름이 암호화되었는지 여부를 나타내는 값.
### getArchiveFormatInfo(InputStream stream) {#getArchiveFormatInfo-java.io.InputStream-}
```
public static ArchiveFormatInfo getArchiveFormatInfo(InputStream stream)
```


아카이브 형식 정보를 가져옵니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 스트림 | java.io.InputStream | 아카이브 파일의 스트림입니다. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format.
### getArchiveFormatInfo(String fileName) {#getArchiveFormatInfo-java.lang.String-}
```
public static ArchiveFormatInfo getArchiveFormatInfo(String fileName)
```


아카이브 형식 정보를 가져옵니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| fileName | java.lang.String | 아카이브 파일의 파일 이름입니다. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format.
### getArchiveInstanceInfo(InputStream stream) {#getArchiveInstanceInfo-java.io.InputStream-}
```
public static ArchiveInstanceInfo getArchiveInstanceInfo(InputStream stream)
```


아카이브 인스턴스 정보를 가져옵니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 스트림 | java.io.InputStream | 아카이브 파일의 스트림입니다. |

**Returns:**
[ArchiveInstanceInfo](../../com.aspose.zip/archiveinstanceinfo) - Information about archive instance or null if format was not detected.
### getArchiveInstanceInfo(String fileName) {#getArchiveInstanceInfo-java.lang.String-}
```
public static ArchiveInstanceInfo getArchiveInstanceInfo(String fileName)
```


아카이브 인스턴스 정보를 가져옵니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| fileName | java.lang.String | 아카이브 파일의 파일 이름입니다. |

**Returns:**
[ArchiveInstanceInfo](../../com.aspose.zip/archiveinstanceinfo) - Information about archive instance or null if format was not detected.
### getFormatInfo() {#getFormatInfo--}
```
public final ArchiveFormatInfo getFormatInfo()
```


아카이브 형식 정보를 가져옵니다.

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - the archive format info.
### isContentEncrypted() {#isContentEncrypted--}
```
public final boolean isContentEncrypted()
```


아카이브 내용이 암호화되었는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 아카이브 내용이 암호화되었는지 여부를 나타내는 값.
