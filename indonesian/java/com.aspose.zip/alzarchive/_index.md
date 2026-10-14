---
title: "AlzArchive"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Mewakili file arsip ALZ."
type: docs
weight: 11
url: /id/java/com.aspose.zip/alzarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class AlzArchive implements IArchive, AutoCloseable
```

Mewakili file arsip ALZ. Gunakan kelas ini untuk memeriksa dan mengekstrak arsip ALZ.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [AlzArchive(InputStream stream)](#AlzArchive-java.io.InputStream-) | Menginisialisasi arsip ALZ dari aliran. |
| [AlzArchive(InputStream stream, AlzArchiveLoadOptions loadOptions)](#AlzArchive-java.io.InputStream-com.aspose.zip.AlzArchiveLoadOptions-) | Menginisialisasi arsip ALZ dari aliran menggunakan opsi pemuatan yang disediakan. |
| [AlzArchive(String filePath)](#AlzArchive-java.lang.String-) | Menginisialisasi arsip ALZ dari jalur file. |
| [AlzArchive(String filePath, AlzArchiveLoadOptions loadOptions)](#AlzArchive-java.lang.String-com.aspose.zip.AlzArchiveLoadOptions-) | Menginisialisasi arsip ALZ dari jalur file menggunakan opsi pemuatan yang disediakan. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [close()](#close--) | Melepaskan sumber daya yang dimiliki oleh arsip ini. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Mengekstrak semua file dan direktori ke direktori yang disediakan. |
| [getEntries()](#getEntries--) | Mendapatkan entri yang membentuk arsip ini. |
| [getFileEntries()](#getFileEntries--) | Mendapatkan entri melalui antarmuka arsip umum. |
| [getFormat()](#getFormat--) | Mendapatkan format arsip. |
### AlzArchive(InputStream stream) {#AlzArchive-java.io.InputStream-}
```
public AlzArchive(InputStream stream)
```


Menginisialisasi arsip ALZ dari aliran.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | java.io.InputStream | Aliran arsip ALZ; harus mendukung pembacaan dan pencarian |

### AlzArchive(InputStream stream, AlzArchiveLoadOptions loadOptions) {#AlzArchive-java.io.InputStream-com.aspose.zip.AlzArchiveLoadOptions-}
```
public AlzArchive(InputStream stream, AlzArchiveLoadOptions loadOptions)
```


Menginisialisasi arsip ALZ dari aliran menggunakan opsi pemuatan yang disediakan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | java.io.InputStream | Aliran arsip ALZ; harus mendukung pembacaan dan pencarian |
| loadOptions | [AlzArchiveLoadOptions](../../com.aspose.zip/alzarchiveloadoptions) | opsi yang digunakan untuk memuat arsip |

### AlzArchive(String filePath) {#AlzArchive-java.lang.String-}
```
public AlzArchive(String filePath)
```


Menginisialisasi arsip ALZ dari jalur file.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| filePath | java.lang.String | jalur ke arsip ALZ |

### AlzArchive(String filePath, AlzArchiveLoadOptions loadOptions) {#AlzArchive-java.lang.String-com.aspose.zip.AlzArchiveLoadOptions-}
```
public AlzArchive(String filePath, AlzArchiveLoadOptions loadOptions)
```


Menginisialisasi arsip ALZ dari jalur file menggunakan opsi pemuatan yang disediakan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| filePath | java.lang.String | jalur ke arsip ALZ |
| loadOptions | [AlzArchiveLoadOptions](../../com.aspose.zip/alzarchiveloadoptions) | opsi yang digunakan untuk memuat arsip |

### close() {#close--}
```
public void close()
```


Melepaskan sumber daya yang dimiliki oleh arsip ini.

### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Mengekstrak semua file dan direktori ke direktori yang disediakan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| destinationDirectory | java.lang.String | direktori tujuan; dibuat bila diperlukan |

### getEntries() {#getEntries--}
```
public final List<AlzEntry> getEntries()
```


Mendapatkan entri yang membentuk arsip ini.

**Returns:**
java.util.List&lt;com.aspose.zip.AlzEntry&gt; - daftar tak dapat diubah dari entri ALZ
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Mendapatkan entri melalui antarmuka arsip umum.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entri arsip
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Mendapatkan format arsip.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - [ArchiveFormat.Alz](../../com.aspose.zip/archiveformat\#Alz)
