---
title: "ArchiveInstanceInfo"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Arşiv örneği hakkında bilgi temsil eder."
type: docs
weight: 34
url: /tr/java/com.aspose.zip/archiveinstanceinfo/
---

**Inheritance:**
java.lang.Object
```
public final class ArchiveInstanceInfo
```

Arşiv örneği hakkında bilgi temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [areFileNamesEncrypted()](#areFileNamesEncrypted--) | Arşivin giriş (dosya) adlarının şifrelenip şifrelenmediğini gösteren bir değer alır. |
| [getArchiveFormatInfo(InputStream stream)](#getArchiveFormatInfo-java.io.InputStream-) | Arşiv formatı bilgilerini alır. |
| [getArchiveFormatInfo(String fileName)](#getArchiveFormatInfo-java.lang.String-) | Arşiv formatı bilgilerini alır. |
| [getArchiveInstanceInfo(InputStream stream)](#getArchiveInstanceInfo-java.io.InputStream-) | Arşiv örneği bilgilerini alır. |
| [getArchiveInstanceInfo(String fileName)](#getArchiveInstanceInfo-java.lang.String-) | Arşiv örneği bilgilerini alır. |
| [getFormatInfo()](#getFormatInfo--) | Arşiv formatı bilgisini alır. |
| [isContentEncrypted()](#isContentEncrypted--) | Arşivin içeriğinin şifrelenip şifrelenmediğini gösteren bir değer alır. |
### areFileNamesEncrypted() {#areFileNamesEncrypted--}
```
public final boolean areFileNamesEncrypted()
```


Arşivin giriş (dosya) adlarının şifrelenip şifrelenmediğini gösteren bir değer alır.

**Returns:**
boolean - arşivin giriş (dosya) adlarının şifrelenip şifrelenmediğini gösteren bir değer.
### getArchiveFormatInfo(InputStream stream) {#getArchiveFormatInfo-java.io.InputStream-}
```
public static ArchiveFormatInfo getArchiveFormatInfo(InputStream stream)
```


Arşiv formatı bilgilerini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | java.io.InputStream | Arşiv dosyasının akışı. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format.
### getArchiveFormatInfo(String fileName) {#getArchiveFormatInfo-java.lang.String-}
```
public static ArchiveFormatInfo getArchiveFormatInfo(String fileName)
```


Arşiv formatı bilgilerini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileName | java.lang.String | Arşiv dosyasının dosya adı. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format.
### getArchiveInstanceInfo(InputStream stream) {#getArchiveInstanceInfo-java.io.InputStream-}
```
public static ArchiveInstanceInfo getArchiveInstanceInfo(InputStream stream)
```


Arşiv örneği bilgilerini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | java.io.InputStream | Arşiv dosyasının akışı. |

**Returns:**
[ArchiveInstanceInfo](../../com.aspose.zip/archiveinstanceinfo) - Information about archive instance or null if format was not detected.
### getArchiveInstanceInfo(String fileName) {#getArchiveInstanceInfo-java.lang.String-}
```
public static ArchiveInstanceInfo getArchiveInstanceInfo(String fileName)
```


Arşiv örneği bilgilerini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileName | java.lang.String | Arşiv dosyasının dosya adı. |

**Returns:**
[ArchiveInstanceInfo](../../com.aspose.zip/archiveinstanceinfo) - Information about archive instance or null if format was not detected.
### getFormatInfo() {#getFormatInfo--}
```
public final ArchiveFormatInfo getFormatInfo()
```


Arşiv formatı bilgisini alır.

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - the archive format info.
### isContentEncrypted() {#isContentEncrypted--}
```
public final boolean isContentEncrypted()
```


Arşivin içeriğinin şifrelenip şifrelenmediğini gösteren bir değer alır.

**Returns:**
boolean - arşivin içeriğinin şifrelenip şifrelenmediğini gösteren bir değer.
