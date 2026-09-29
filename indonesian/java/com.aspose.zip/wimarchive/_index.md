---
title: "WimArchive"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Kelas ini mewakili file arsip wim."
type: docs
weight: 130
url: /id/java/com.aspose.zip/wimarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class WimArchive implements IArchive, AutoCloseable
```

Kelas ini mewakili file arsip wim.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [WimArchive(InputStream sourceStream)](#WimArchive-java.io.InputStream-) | Menginisialisasi sebuah instance baru dari kelas [WimArchive](../../com.aspose.zip/wimarchive) dan menyusun daftar entri yang dapat diekstrak dari arsip. |
| [WimArchive(InputStream sourceStream, WimLoadOptions loadOptions)](#WimArchive-java.io.InputStream-com.aspose.zip.WimLoadOptions-) | Menginisialisasi sebuah instance baru dari kelas [WimArchive](../../com.aspose.zip/wimarchive) dan menyusun daftar entri yang dapat diekstrak dari arsip. |
| [WimArchive(String path)](#WimArchive-java.lang.String-) | Menginisialisasi sebuah instance baru dari kelas [WimArchive](../../com.aspose.zip/wimarchive) dan menyusun daftar entri yang dapat diekstrak dari arsip. |
| [WimArchive(String path, WimLoadOptions loadOptions)](#WimArchive-java.lang.String-com.aspose.zip.WimLoadOptions-) | Menginisialisasi sebuah instance baru dari kelas [WimArchive](../../com.aspose.zip/wimarchive) dan menyusun daftar entri yang dapat diekstrak dari arsip. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Mengekstrak arsip ke file berdasarkan jalur. |
| [getBootImageIndex()](#getBootImageIndex--) | Mendapatkan indeks (berbasis nol) dari gambar yang dapat di-boot. |
| [getEntries()](#getEntries--) | Mendapatkan entri tipe [WimEntry](../../com.aspose.zip/wimentry) yang membentuk arsip. |
| [getFileEntries()](#getFileEntries--) | Mendapatkan entri tipe [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) yang membentuk arsip wim. |
| [getFileFormatVersion()](#getFileFormatVersion--) | Mendapatkan versi format file. |
| [getFormat()](#getFormat--) | Mendapatkan format arsip. |
| [getGuid()](#getGuid--) | Mendapatkan UUID identifikasi untuk arsip. |
| [getImages()](#getImages--) | Mendapatkan entri tipe [WimImage](../../com.aspose.zip/wimimage) yang membentuk arsip. |
| [getManifest()](#getManifest--) | Mendapatkan manifes tersemat yang menggambarkan file dan gambar yang terkandung. |
### WimArchive(InputStream sourceStream) {#WimArchive-java.io.InputStream-}
```
public WimArchive(InputStream sourceStream)
```


Menginisialisasi sebuah instance baru dari kelas [WimArchive](../../com.aspose.zip/wimarchive) dan menyusun daftar entri yang dapat diekstrak dari arsip.

Contoh berikut menunjukkan cara mengekstrak semua entri ke sebuah direktori.

```

``````

try (WimArchive archive = new WimArchive(new FileInputStream("archive.wim"))) {
archive.getImages().get_Item(0).extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry. See [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |

### WimArchive(InputStream sourceStream, WimLoadOptions loadOptions) {#WimArchive-java.io.InputStream-com.aspose.zip.WimLoadOptions-}
```
public WimArchive(InputStream sourceStream, WimLoadOptions loadOptions)
```


Initializes a new instance of the [WimArchive](../../com.aspose.zip/wimarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all of the entries to a directory.

```

``````

     try (WimArchive archive = new WimArchive(new FileInputStream("archive.wim"))) {
         archive.getImages().get_Item(0).extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

Konstruktor ini tidak mengekstrak entri apa pun. Lihat metode [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\#open--) untuk mengekstrak.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| sourceStream | java.io.InputStream | sumber arsip |
| loadOptions | [WimLoadOptions](../../com.aspose.zip/wimloadoptions) | Opsi untuk memuat arsip yang ada. |

### WimArchive(String path) {#WimArchive-java.lang.String-}
```
public WimArchive(String path)
```


Menginisialisasi sebuah instance baru dari kelas [WimArchive](../../com.aspose.zip/wimarchive) dan menyusun daftar entri yang dapat diekstrak dari arsip.

Contoh berikut menunjukkan cara mengekstrak semua entri ke sebuah direktori.

```

``````

try (WimArchive archive = new WimArchive("archive.wim")) {
archive.getImages().get_Item(0).extractToDirectory("C:\\extracted");
}
 
```

This constructor does not unpack any entry. See [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### WimArchive(String path, WimLoadOptions loadOptions) {#WimArchive-java.lang.String-com.aspose.zip.WimLoadOptions-}
```
public WimArchive(String path, WimLoadOptions loadOptions)
```


Initializes a new instance of the [WimArchive](../../com.aspose.zip/wimarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all of the entries to a directory.

```

``````

     try (WimArchive archive = new WimArchive("archive.wim")) {
         archive.getImages().get_Item(0).extractToDirectory("C:\\extracted");
     }
 
```

Konstruktor ini tidak mengekstrak entri apa pun. Lihat metode [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\#open--) untuk mengekstrak.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | java.lang.String | jalur ke file arsip |
| loadOptions | [WimLoadOptions](../../com.aspose.zip/wimloadoptions) | Opsi untuk memuat arsip yang ada. |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Mengekstrak arsip ke file berdasarkan jalur.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| destinationDirectory | java.lang.String | jalur ke direktori tempat menempatkan file yang diekstrak |

### getBootImageIndex() {#getBootImageIndex--}
```
public final int getBootImageIndex()
```


Mendapatkan indeks (berbasis nol) dari gambar yang dapat di-boot.

**Returns:**
int - indeks (berbasis nol) dari gambar yang dapat di-boot
### getEntries() {#getEntries--}
```
public final List<WimEntry> getEntries()
```


Mendapatkan entri tipe [WimEntry](../../com.aspose.zip/wimentry) yang membentuk arsip.

**Returns:**
java.util.List&lt;com.aspose.zip.WimEntry&gt; - entri yang membentuk arsip
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Mendapatkan entri tipe [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) yang membentuk arsip wim.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entri tipe [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) yang membentuk arsip wim
### getFileFormatVersion() {#getFileFormatVersion--}
```
public final int getFileFormatVersion()
```


Mendapatkan versi format file.

**Returns:**
int - versi format file
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Mendapatkan format arsip.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getGuid() {#getGuid--}
```
public final UUID getGuid()
```


Mendapatkan UUID identifikasi untuk arsip.

**Returns:**
java.util.UUID - UUID yang mengidentifikasi arsip
### getImages() {#getImages--}
```
public final List<WimImage> getImages()
```


Mendapatkan entri tipe [WimImage](../../com.aspose.zip/wimimage) yang membentuk arsip.

**Returns:**
java.util.List&lt;com.aspose.zip.WimImage&gt; - entri tipe [WimImage](../../com.aspose.zip/wimimage) yang membentuk arsip
### getManifest() {#getManifest--}
```
public final String getManifest()
```


Mendapatkan manifes tersemat yang menggambarkan file dan gambar yang terkandung.

**Returns:**
java.lang.String - manifest tersemat yang menjelaskan file dan gambar yang terkandung
