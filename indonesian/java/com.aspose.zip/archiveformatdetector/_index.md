---
title: "ArchiveFormatDetector"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Mendeteksi format arsip dan menyediakan informasi terkait lainnya."
type: docs
weight: 32
url: /id/java/com.aspose.zip/archiveformatdetector/
---

**Inheritance:**
java.lang.Object
```
public final class ArchiveFormatDetector
```

Mendeteksi format arsip dan menyediakan informasi terkait lainnya.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [ArchiveFormatDetector()](#ArchiveFormatDetector--) | Menginisialisasi instance baru dari kelas [ArchiveFormatDetector](../../com.aspose.zip/archiveformatdetector). |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getFormatInfo(InputStream stream)](#getFormatInfo-java.io.InputStream-) | Mendapatkan info format. |
| [getFormatInfo(String fileName)](#getFormatInfo-java.lang.String-) | Mendapatkan info format. |
### ArchiveFormatDetector() {#ArchiveFormatDetector--}
```
public ArchiveFormatDetector()
```


Menginisialisasi instance baru dari kelas [ArchiveFormatDetector](../../com.aspose.zip/archiveformatdetector).

### getFormatInfo(InputStream stream) {#getFormatInfo-java.io.InputStream-}
```
public final ArchiveFormatInfo getFormatInfo(InputStream stream)
```


Mendapatkan info format.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | java.io.InputStream | Stream dari file arsip. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format or null if a format was not detected.
### getFormatInfo(String fileName) {#getFormatInfo-java.lang.String-}
```
public final ArchiveFormatInfo getFormatInfo(String fileName)
```


Mendapatkan info format.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fileName | java.lang.String | Nama file dari file arsip. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format or null if a format was not detected.
