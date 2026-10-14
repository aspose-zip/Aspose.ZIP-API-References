---
title: "ArchiveFormatDetector"
second_title: "Aspose.ZIP for Java API 참조"
description: "아카이브 형식을 감지하고 기타 관련 정보를 제공합니다."
type: docs
weight: 32
url: /ko/java/com.aspose.zip/archiveformatdetector/
---

**Inheritance:**
java.lang.Object
```
public final class ArchiveFormatDetector
```

아카이브 형식을 감지하고 기타 관련 정보를 제공합니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [ArchiveFormatDetector()](#ArchiveFormatDetector--) | 새로운 [ArchiveFormatDetector](../../com.aspose.zip/archiveformatdetector) 클래스 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getFormatInfo(InputStream stream)](#getFormatInfo-java.io.InputStream-) | 형식 정보를 가져옵니다. |
| [getFormatInfo(String fileName)](#getFormatInfo-java.lang.String-) | 형식 정보를 가져옵니다. |
### ArchiveFormatDetector() {#ArchiveFormatDetector--}
```
public ArchiveFormatDetector()
```


새로운 [ArchiveFormatDetector](../../com.aspose.zip/archiveformatdetector) 클래스 인스턴스를 초기화합니다.

### getFormatInfo(InputStream stream) {#getFormatInfo-java.io.InputStream-}
```
public final ArchiveFormatInfo getFormatInfo(InputStream stream)
```


형식 정보를 가져옵니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 스트림 | java.io.InputStream | 아카이브 파일의 스트림입니다. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format or null if a format was not detected.
### getFormatInfo(String fileName) {#getFormatInfo-java.lang.String-}
```
public final ArchiveFormatInfo getFormatInfo(String fileName)
```


형식 정보를 가져옵니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| fileName | java.lang.String | 아카이브 파일의 파일 이름입니다. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format or null if a format was not detected.
