---
title: "ArchiveInstanceInfo"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Mewakili informasi tentang instansi arsip."
type: docs
weight: 34
url: /id/java/com.aspose.zip/archiveinstanceinfo/
---

**Inheritance:**
java.lang.Object
```
public final class ArchiveInstanceInfo
```

Mewakili informasi tentang instansi arsip.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [areFileNamesEncrypted()](#areFileNamesEncrypted--) | Mendapatkan nilai yang menunjukkan apakah nama entri (file) dalam arsip dienkripsi. |
| [getArchiveFormatInfo(InputStream stream)](#getArchiveFormatInfo-java.io.InputStream-) | Mendapatkan info format arsip. |
| [getArchiveFormatInfo(String fileName)](#getArchiveFormatInfo-java.lang.String-) | Mendapatkan info format arsip. |
| [getArchiveInstanceInfo(InputStream stream)](#getArchiveInstanceInfo-java.io.InputStream-) | Mendapatkan info instance arsip. |
| [getArchiveInstanceInfo(String fileName)](#getArchiveInstanceInfo-java.lang.String-) | Mendapatkan info instance arsip. |
| [getFormatInfo()](#getFormatInfo--) | Mendapatkan info format arsip. |
| [isContentEncrypted()](#isContentEncrypted--) | Mendapatkan nilai yang menunjukkan apakah konten arsip dienkripsi. |
### areFileNamesEncrypted() {#areFileNamesEncrypted--}
```
public final boolean areFileNamesEncrypted()
```


Mendapatkan nilai yang menunjukkan apakah nama entri (file) dalam arsip dienkripsi.

**Returns:**
boolean - nilai yang menunjukkan apakah nama entri (file) arsip dienkripsi.
### getArchiveFormatInfo(InputStream stream) {#getArchiveFormatInfo-java.io.InputStream-}
```
public static ArchiveFormatInfo getArchiveFormatInfo(InputStream stream)
```


Mendapatkan info format arsip.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | java.io.InputStream | Stream dari file arsip. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format.
### getArchiveFormatInfo(String fileName) {#getArchiveFormatInfo-java.lang.String-}
```
public static ArchiveFormatInfo getArchiveFormatInfo(String fileName)
```


Mendapatkan info format arsip.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fileName | java.lang.String | Nama file dari file arsip. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format.
### getArchiveInstanceInfo(InputStream stream) {#getArchiveInstanceInfo-java.io.InputStream-}
```
public static ArchiveInstanceInfo getArchiveInstanceInfo(InputStream stream)
```


Mendapatkan info instance arsip.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | java.io.InputStream | Stream dari file arsip. |

**Returns:**
[ArchiveInstanceInfo](../../com.aspose.zip/archiveinstanceinfo) - Information about archive instance or null if format was not detected.
### getArchiveInstanceInfo(String fileName) {#getArchiveInstanceInfo-java.lang.String-}
```
public static ArchiveInstanceInfo getArchiveInstanceInfo(String fileName)
```


Mendapatkan info instance arsip.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fileName | java.lang.String | Nama file dari file arsip. |

**Returns:**
[ArchiveInstanceInfo](../../com.aspose.zip/archiveinstanceinfo) - Information about archive instance or null if format was not detected.
### getFormatInfo() {#getFormatInfo--}
```
public final ArchiveFormatInfo getFormatInfo()
```


Mendapatkan info format arsip.

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - the archive format info.
### isContentEncrypted() {#isContentEncrypted--}
```
public final boolean isContentEncrypted()
```


Mendapatkan nilai yang menunjukkan apakah konten arsip dienkripsi.

**Returns:**
boolean - nilai yang menunjukkan apakah konten arsip dienkripsi.
