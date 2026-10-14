---
title: "LhaArchive"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Kelas ini mewakili file arsip LHA .lzh."
type: docs
weight: 75
url: /id/java/com.aspose.zip/lhaarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class LhaArchive implements IArchive, AutoCloseable
```

Kelas ini mewakili file arsip LHA (.lzh).

Hanya metode kompresi berikut yang didukung:

| ------ | --------------------------------------------- |
| Method | Explanation                                   |
| lh0    | Tidak terkompresi                                  |
| lh4    | 8 KiB kamus geser dan Huffman statis   |
| lh5    | 16 KiB kamus geser dan Huffman statis  |
| lh6    | 64 KiB kamus geser dan Huffman statis  |
| lh7    | 128 KiB kamus geser dan Huffman statis |
| lhx    | 1 Mib kamus geser dan Huffman statis   |
| lhd    | Direktori                                     |
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [LhaArchive(InputStream sourceStream)](#LhaArchive-java.io.InputStream-) | Menginisialisasi instance baru dari kelas [LhaArchive](../../com.aspose.zip/lhaarchive) dan menyusun daftar entri yang dapat diekstrak dari arsip. |
| [LhaArchive(InputStream sourceStream, LhaLoadOptions loadOptions)](#LhaArchive-java.io.InputStream-com.aspose.zip.LhaLoadOptions-) | Menginisialisasi instance baru dari kelas [LhaArchive](../../com.aspose.zip/lhaarchive) dan menyusun daftar entri yang dapat diekstrak dari arsip. |
| [LhaArchive(String path)](#LhaArchive-java.lang.String-) | Menginisialisasi instance baru dari kelas [LhaArchive](../../com.aspose.zip/lhaarchive) dan menyusun daftar entri yang dapat diekstrak dari arsip. |
| [LhaArchive(String path, LhaLoadOptions loadOptions)](#LhaArchive-java.lang.String-com.aspose.zip.LhaLoadOptions-) | Menginisialisasi instance baru dari kelas [LhaArchive](../../com.aspose.zip/lhaarchive) dan menyusun daftar entri yang dapat diekstrak dari arsip. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Mengekstrak semua file dan direktori dalam arsip ke direktori yang diberikan. |
| [getEntries()](#getEntries--) | Mendapatkan entri file bertipe [LhaArchiveEntry](../../com.aspose.zip/lhaarchiveentry) yang membentuk arsip. |
| [getFileEntries()](#getFileEntries--) | Mendapatkan entri tipe [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) yang membentuk arsip. |
| [getFormat()](#getFormat--) | Mendapatkan format arsip. |
### LhaArchive(InputStream sourceStream) {#LhaArchive-java.io.InputStream-}
```
public LhaArchive(InputStream sourceStream)
```


Menginisialisasi instance baru dari kelas [LhaArchive](../../com.aspose.zip/lhaarchive) dan menyusun daftar entri yang dapat diekstrak dari arsip.

Konstruktor ini tidak mendekompresi entri apa pun. Lihat metode [LhaArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lhaarchiveentry\#extract-OutputStream-) untuk mendekompresi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| sourceStream | java.io.InputStream | sumber arsip |

### LhaArchive(InputStream sourceStream, LhaLoadOptions loadOptions) {#LhaArchive-java.io.InputStream-com.aspose.zip.LhaLoadOptions-}
```
public LhaArchive(InputStream sourceStream, LhaLoadOptions loadOptions)
```


Menginisialisasi instance baru dari kelas [LhaArchive](../../com.aspose.zip/lhaarchive) dan menyusun daftar entri yang dapat diekstrak dari arsip.

Konstruktor ini tidak mendekompresi entri apa pun. Lihat metode [LhaArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lhaarchiveentry\#extract-OutputStream-) untuk mendekompresi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| sourceStream | java.io.InputStream | sumber arsip |
| loadOptions | [LhaLoadOptions](../../com.aspose.zip/lhaloadoptions) | Opsi untuk memuat arsip yang ada. |

### LhaArchive(String path) {#LhaArchive-java.lang.String-}
```
public LhaArchive(String path)
```


Menginisialisasi instance baru dari kelas [LhaArchive](../../com.aspose.zip/lhaarchive) dan menyusun daftar entri yang dapat diekstrak dari arsip.

Contoh berikut mengekstrak sebuah arsip, kemudian mendekompresi entri pertama ke `MemoryStream`.

```

``````

ByteArrayOutputStream extracted = new ByteArrayOutputStream();
try (LhaArchive archive = new LhaArchive("sample.lzh")) {
archive.getEntries().get(0).extract(extracted);
}
 
```

This constructor does not decompress any entry. See [ArchiveEntry.extract(OutputStream)](../../com.aspose.zip/archiveentry\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the fully qualified or the relative path to the archive file |

### LhaArchive(String path, LhaLoadOptions loadOptions) {#LhaArchive-java.lang.String-com.aspose.zip.LhaLoadOptions-}
```
public LhaArchive(String path, LhaLoadOptions loadOptions)
```


Initializes a new instance of the [LhaArchive](../../com.aspose.zip/lhaarchive) class and composes an entry list can be extracted from the archive.

The following example extracts an archive, then decompress first entry to a `MemoryStream`.

```

``````

     ByteArrayOutputStream extracted = new ByteArrayOutputStream();
     try (LhaArchive archive = new LhaArchive("sample.lzh")) {
         archive.getEntries().get(0).extract(extracted);
     }
 
```

Konstruktor ini tidak mendekompresi entri apa pun. Lihat metode [ArchiveEntry.extract(OutputStream)](../../com.aspose.zip/archiveentry\#extract-OutputStream-) untuk mendekompresi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | java.lang.String | jalur yang sepenuhnya memenuhi syarat atau jalur relatif ke file arsip |
| loadOptions | [LhaLoadOptions](../../com.aspose.zip/lhaloadoptions) | Opsi untuk memuat arsip yang ada. |

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

try (LhaArchive archive = new LhaArchive("archive.lzh")) {
archive.extractToDirectory("C:/extracted");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in.

If the directory does not exist, it will be created |

### getEntries() {#getEntries--}
```
public final List<LhaArchiveEntry> getEntries()
```


Gets file entries of [LhaArchiveEntry](../../com.aspose.zip/lhaarchiveentry) type constituting the archive.

**Returns:**
java.util.List&lt;com.aspose.zip.LhaArchiveEntry&gt; - file entries of [LhaArchiveEntry](../../com.aspose.zip/lhaarchiveentry) type constituting the archive
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
