---
title: "LzxArchive"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Kelas ini mewakili file arsip LZX .lzx."
type: docs
weight: 89
url: /id/java/com.aspose.zip/lzxarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class LzxArchive implements IArchive, AutoCloseable
```

Kelas ini mewakili file arsip LZX (.lzx).
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [LzxArchive(InputStream extractionSource)](#LzxArchive-java.io.InputStream-) | Menginisialisasi sebuah instance baru dari kelas [LzxArchive](../../com.aspose.zip/lzxarchive) dan menyusun daftar entri yang dapat diekstrak dari arsip. |
| [LzxArchive(InputStream extractionSource, LzxLoadOptions loadOptions)](#LzxArchive-java.io.InputStream-com.aspose.zip.LzxLoadOptions-) | Menginisialisasi sebuah instance baru dari kelas [LzxArchive](../../com.aspose.zip/lzxarchive) dan menyusun daftar entri yang dapat diekstrak dari arsip. |
| [LzxArchive(String path)](#LzxArchive-java.lang.String-) | Menginisialisasi sebuah instance baru dari kelas [LzxArchive](../../com.aspose.zip/lzxarchive) dan menyusun daftar entri yang dapat diekstrak dari arsip. |
| [LzxArchive(String path, LzxLoadOptions loadOptions)](#LzxArchive-java.lang.String-com.aspose.zip.LzxLoadOptions-) | Menginisialisasi sebuah instance baru dari kelas [LzxArchive](../../com.aspose.zip/lzxarchive) dan menyusun daftar entri yang dapat diekstrak dari arsip. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Mengekstrak semua file dan direktori dalam arsip ke direktori yang diberikan. |
| [getEntries()](#getEntries--) | Mendapatkan entri file bertipe [LzxArchiveEntry](../../com.aspose.zip/lzxarchiveentry) yang membentuk arsip. |
| [getFileEntries()](#getFileEntries--) | Mendapatkan entri tipe [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) yang membentuk arsip. |
| [getFormat()](#getFormat--) | Mendapatkan format arsip. |
### LzxArchive(InputStream extractionSource) {#LzxArchive-java.io.InputStream-}
```
public LzxArchive(InputStream extractionSource)
```


Menginisialisasi sebuah instance baru dari kelas [LzxArchive](../../com.aspose.zip/lzxarchive) dan menyusun daftar entri yang dapat diekstrak dari arsip.

Konstruktor ini tidak mendekompresi entri apa pun. Lihat metode [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\#extract-OutputStream-) untuk mendekompresi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| extractionSource | java.io.InputStream | Sumber arsip. |

### LzxArchive(InputStream extractionSource, LzxLoadOptions loadOptions) {#LzxArchive-java.io.InputStream-com.aspose.zip.LzxLoadOptions-}
```
public LzxArchive(InputStream extractionSource, LzxLoadOptions loadOptions)
```


Menginisialisasi sebuah instance baru dari kelas [LzxArchive](../../com.aspose.zip/lzxarchive) dan menyusun daftar entri yang dapat diekstrak dari arsip.

Konstruktor ini tidak mendekompresi entri apa pun. Lihat metode [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\#extract-OutputStream-) untuk mendekompresi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| extractionSource | java.io.InputStream | Sumber arsip. |
| loadOptions | [LzxLoadOptions](../../com.aspose.zip/lzxloadoptions) | Opsi untuk memuat arsip yang ada. |

### LzxArchive(String path) {#LzxArchive-java.lang.String-}
```
public LzxArchive(String path)
```


Menginisialisasi sebuah instance baru dari kelas [LzxArchive](../../com.aspose.zip/lzxarchive) dan menyusun daftar entri yang dapat diekstrak dari arsip.

Contoh berikut mengekstrak sebuah arsip, kemudian mendekompresi entri pertama ke `MemoryStream`.

```

``````

ByteArrayOutputStream extracted = new ByteArrayOutputStream();
try (LzxArchive archive = new LzxArchive("sample.lzx")) {
archive.getEntries().get(0).extract(extracted);
}
 
```

This constructor does not decompress any entry. See [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The fully qualified or the relative path to the archive file. |

### LzxArchive(String path, LzxLoadOptions loadOptions) {#LzxArchive-java.lang.String-com.aspose.zip.LzxLoadOptions-}
```
public LzxArchive(String path, LzxLoadOptions loadOptions)
```


Initializes a new instance of the [LzxArchive](../../com.aspose.zip/lzxarchive) class and composes an entry list can be extracted from the archive.

The following example extracts an archive, then decompress first entry to a `MemoryStream`.

```

``````

     ByteArrayOutputStream extracted = new ByteArrayOutputStream();
     try (LzxArchive archive = new LzxArchive("sample.lzx")) {
         archive.getEntries().get(0).extract(extracted);
     }
 
```

Konstruktor ini tidak mendekompresi entri apa pun. Lihat metode [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\#extract-OutputStream-) untuk mendekompresi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | java.lang.String | Jalur lengkap atau jalur relatif ke file arsip. |
| loadOptions | [LzxLoadOptions](../../com.aspose.zip/lzxloadoptions) | Opsi untuk memuat arsip yang ada. |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Mengekstrak semua file dan direktori dalam arsip ke direktori yang diberikan.

```

``````

try (LzxArchive archive = new LzxArchive("archive.lzx")) {
archive.extractToDirectory("C:/extracted");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | The path to the directory to place the extracted files in.

If the directory does not exist, it will be created. |

### getEntries() {#getEntries--}
```
public final List<LzxArchiveEntry> getEntries()
```


Gets file entries of [LzxArchiveEntry](../../com.aspose.zip/lzxarchiveentry) type constituting the archive.

**Returns:**
java.util.List&lt;com.aspose.zip.LzxArchiveEntry&gt; - file entries of [LzxArchiveEntry](../../com.aspose.zip/lzxarchiveentry) type constituting the archive.
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the archive
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Gets the archive format.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
