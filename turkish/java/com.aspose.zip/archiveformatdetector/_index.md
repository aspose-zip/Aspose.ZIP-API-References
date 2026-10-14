---
title: "ArchiveFormatDetector"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Bir arşiv formatını algılar ve diğer ilgili bilgileri sağlar."
type: docs
weight: 32
url: /tr/java/com.aspose.zip/archiveformatdetector/
---

**Inheritance:**
java.lang.Object
```
public final class ArchiveFormatDetector
```

Bir arşiv formatını algılar ve diğer ilgili bilgileri sağlar.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [ArchiveFormatDetector()](#ArchiveFormatDetector--) | Yeni bir [ArchiveFormatDetector](../../com.aspose.zip/archiveformatdetector) sınıfı örneği başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getFormatInfo(InputStream stream)](#getFormatInfo-java.io.InputStream-) | Biçim bilgilerini alır. |
| [getFormatInfo(String fileName)](#getFormatInfo-java.lang.String-) | Biçim bilgilerini alır. |
### ArchiveFormatDetector() {#ArchiveFormatDetector--}
```
public ArchiveFormatDetector()
```


Yeni bir [ArchiveFormatDetector](../../com.aspose.zip/archiveformatdetector) sınıfı örneği başlatır.

### getFormatInfo(InputStream stream) {#getFormatInfo-java.io.InputStream-}
```
public final ArchiveFormatInfo getFormatInfo(InputStream stream)
```


Biçim bilgilerini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | java.io.InputStream | Arşiv dosyasının akışı. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format or null if a format was not detected.
### getFormatInfo(String fileName) {#getFormatInfo-java.lang.String-}
```
public final ArchiveFormatInfo getFormatInfo(String fileName)
```


Biçim bilgilerini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileName | java.lang.String | Arşiv dosyasının dosya adı. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format or null if a format was not detected.
