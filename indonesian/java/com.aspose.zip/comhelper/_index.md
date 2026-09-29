---
title: "ComHelper"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Menyediakan metode untuk klien COM agar memuat arsip ke dalam Aspose.Zip."
type: docs
weight: 55
url: /id/java/com.aspose.zip/comhelper/
---

**Inheritance:**
java.lang.Object
```
public class ComHelper
```

Menyediakan metode untuk klien COM agar memuat arsip ke dalam Aspose.Zip.

Gunakan kelas ComHelper untuk memuat arsip dari file atau aliran. Kelas tertentu menyediakan konstruktor default untuk membuat arsip baru dan juga menyediakan konstruktor overload untuk memuat arsip dari file atau aliran. Jika Anda menggunakan Aspose.Zip dari aplikasi .NET, Anda dapat menggunakan semua konstruktor arsip secara langsung, tetapi jika Anda menggunakan Aspose.Zip dari aplikasi COM, hanya konstruktor arsip default yang tersedia.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [ComHelper()](#ComHelper--) | Menginisialisasi instance baru dari kelas ini. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [openBzip2(InputStream stream)](#openBzip2-java.io.InputStream-) | Mengizinkan aplikasi COM untuk memuat arsip bzip2 dari aliran. |
| [openBzip2(String fileName)](#openBzip2-java.lang.String-) | Mengizinkan aplikasi COM untuk memuat arsip bzip2 dari file. |
| [openGzip(InputStream stream)](#openGzip-java.io.InputStream-) | Mengizinkan aplikasi COM untuk memuat arsip gzip dari aliran. |
| [openGzip(String fileName)](#openGzip-java.lang.String-) | Mengizinkan aplikasi COM untuk memuat arsip gzip dari file. |
| [openRar(InputStream stream)](#openRar-java.io.InputStream-) | Mengizinkan aplikasi COM untuk memuat arsip rar dari aliran. |
| [openRar(String fileName)](#openRar-java.lang.String-) | Mengizinkan aplikasi COM untuk memuat arsip rar dari file. |
| [openZip(InputStream stream)](#openZip-java.io.InputStream-) | Mengizinkan aplikasi COM untuk memuat arsip ZIP dari aliran. |
| [openZip(String fileName)](#openZip-java.lang.String-) | Mengizinkan aplikasi COM untuk memuat arsip ZIP dari file. |
### ComHelper() {#ComHelper--}
```
public ComHelper()
```


Menginisialisasi instance baru dari kelas ini.

### openBzip2(InputStream stream) {#openBzip2-java.io.InputStream-}
```
public final Bzip2Archive openBzip2(InputStream stream)
```


Mengizinkan aplikasi COM untuk memuat arsip bzip2 dari aliran.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | java.io.InputStream | Objek aliran .NET yang berisi arsip yang akan dimuat. |

**Returns:**
[Bzip2Archive](../../com.aspose.zip/bzip2archive) - A [Bzip2Archive](../../com.aspose.zip/bzip2archive) object that represents the archive.
### openBzip2(String fileName) {#openBzip2-java.lang.String-}
```
public final Bzip2Archive openBzip2(String fileName)
```


Mengizinkan aplikasi COM untuk memuat arsip bzip2 dari file.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fileName | java.lang.String | Nama file arsip yang akan dimuat. |

**Returns:**
[Bzip2Archive](../../com.aspose.zip/bzip2archive) - A [Bzip2Archive](../../com.aspose.zip/bzip2archive) object that represents the archive.
### openGzip(InputStream stream) {#openGzip-java.io.InputStream-}
```
public final GzipArchive openGzip(InputStream stream)
```


Mengizinkan aplikasi COM untuk memuat arsip gzip dari aliran.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | java.io.InputStream | Objek aliran .NET yang berisi arsip yang akan dimuat. |

**Returns:**
[GzipArchive](../../com.aspose.zip/gziparchive) - A [GzipArchive](../../com.aspose.zip/gziparchive) object that represents the archive.
### openGzip(String fileName) {#openGzip-java.lang.String-}
```
public final GzipArchive openGzip(String fileName)
```


Mengizinkan aplikasi COM untuk memuat arsip gzip dari file.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fileName | java.lang.String | Nama file arsip yang akan dimuat. |

**Returns:**
[GzipArchive](../../com.aspose.zip/gziparchive) - A [GzipArchive](../../com.aspose.zip/gziparchive) object that represents the archive.
### openRar(InputStream stream) {#openRar-java.io.InputStream-}
```
public final RarArchive openRar(InputStream stream)
```


Mengizinkan aplikasi COM untuk memuat arsip rar dari aliran.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | java.io.InputStream | Objek aliran .NET yang berisi arsip yang akan dimuat. |

**Returns:**
[RarArchive](../../com.aspose.zip/rararchive) - A [RarArchive](../../com.aspose.zip/rararchive) object that represents the archive.
### openRar(String fileName) {#openRar-java.lang.String-}
```
public final RarArchive openRar(String fileName)
```


Mengizinkan aplikasi COM untuk memuat arsip rar dari file.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fileName | java.lang.String | Nama file arsip yang akan dimuat. |

**Returns:**
[RarArchive](../../com.aspose.zip/rararchive) - A [RarArchive](../../com.aspose.zip/rararchive) object that represents the archive.
### openZip(InputStream stream) {#openZip-java.io.InputStream-}
```
public final Archive openZip(InputStream stream)
```


Mengizinkan aplikasi COM untuk memuat arsip ZIP dari aliran.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | java.io.InputStream | Objek aliran .NET yang berisi arsip yang akan dimuat. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - A [Archive](../../com.aspose.zip/archive) object that represents the archive.
### openZip(String fileName) {#openZip-java.lang.String-}
```
public final Archive openZip(String fileName)
```


Mengizinkan aplikasi COM untuk memuat arsip ZIP dari file.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fileName | java.lang.String | Nama file arsip yang akan dimuat. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - A [Archive](../../com.aspose.zip/archive) object that represents the archive.
