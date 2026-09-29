---
title: "ArjArchive"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Kelas ini mewakili file arsip ARJ."
type: docs
weight: 37
url: /id/java/com.aspose.zip/arjarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class ArjArchive implements IArchive, AutoCloseable
```

Kelas ini mewakili file arsip ARJ.

Hanya metode kompresi berikut yang didukung:

| ------ | ------------------------------------------------------------ |
| Method | Explanation                                                  |
| 0      | Tidak terkompresi                                                 |
| 1      | Kombinasi LZ77 dan pengkodean Huffman adaptif. Rasio terbaik. |
| 2      | Kombinasi LZ77 dan pengkodean Huffman adaptif.             |
| 3      | Kombinasi LZ77 dan pengkodean Huffman adaptif. Kecepatan terbaik. |
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [ArjArchive(InputStream extractionSource)](#ArjArchive-java.io.InputStream-) | Menginisialisasi sebuah instance baru dari kelas [ArjArchive](../../com.aspose.zip/arjarchive) dan menyusun daftar entri yang dapat diekstrak dari arsip. |
| [ArjArchive(InputStream extractionSource, ArjLoadOptions loadOptions)](#ArjArchive-java.io.InputStream-com.aspose.zip.ArjLoadOptions-) | Menginisialisasi sebuah instance baru dari kelas [ArjArchive](../../com.aspose.zip/arjarchive) dan menyusun daftar entri yang dapat diekstrak dari arsip. |
| [ArjArchive(String path)](#ArjArchive-java.lang.String-) | Menginisialisasi sebuah instance baru dari kelas [ArjArchive](../../com.aspose.zip/arjarchive) dan menyusun daftar entri yang dapat diekstrak dari arsip. |
| [ArjArchive(String path, ArjLoadOptions loadOptions)](#ArjArchive-java.lang.String-com.aspose.zip.ArjLoadOptions-) | Menginisialisasi sebuah instance baru dari kelas [ArjArchive](../../com.aspose.zip/arjarchive) dan menyusun daftar entri yang dapat diekstrak dari arsip. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Mengekstrak semua entri ke direktori yang ditentukan. |
| [getCommentary()](#getCommentary--) | Mendapatkan komentar. |
| [getEntries()](#getEntries--) | Mendapatkan entri tipe [ArjEntryPlain](../../com.aspose.zip/arjentryplain) yang membentuk arsip ARJ. |
| [getFileEntries()](#getFileEntries--) | Mendapatkan entri tipe [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) yang membentuk arsip. |
| [getFormat()](#getFormat--) | Mendapatkan format arsip. |
| [getName()](#getName--) | Mendapatkan nama asli. |
### ArjArchive(InputStream extractionSource) {#ArjArchive-java.io.InputStream-}
```
public ArjArchive(InputStream extractionSource)
```


Menginisialisasi sebuah instance baru dari kelas [ArjArchive](../../com.aspose.zip/arjarchive) dan menyusun daftar entri yang dapat diekstrak dari arsip.

Konstruktor ini tidak mendekompresi entri apa pun. Lihat metode [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\\#extract-java.io.OutputStream-) untuk mendekompresi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| extractionSource | java.io.InputStream | sumber arsip |

### ArjArchive(InputStream extractionSource, ArjLoadOptions loadOptions) {#ArjArchive-java.io.InputStream-com.aspose.zip.ArjLoadOptions-}
```
public ArjArchive(InputStream extractionSource, ArjLoadOptions loadOptions)
```


Menginisialisasi sebuah instance baru dari kelas [ArjArchive](../../com.aspose.zip/arjarchive) dan menyusun daftar entri yang dapat diekstrak dari arsip.

Konstruktor ini tidak mendekompresi entri apa pun. Lihat metode [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\\#extract-java.io.OutputStream-) untuk mendekompresi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| extractionSource | java.io.InputStream | sumber arsip |
| loadOptions | [ArjLoadOptions](../../com.aspose.zip/arjloadoptions) | Opsi untuk memuat arsip yang ada. |

### ArjArchive(String path) {#ArjArchive-java.lang.String-}
```
public ArjArchive(String path)
```


Menginisialisasi sebuah instance baru dari kelas [ArjArchive](../../com.aspose.zip/arjarchive) dan menyusun daftar entri yang dapat diekstrak dari arsip.

Contoh berikut menunjukkan cara mengekstrak semua entri ke sebuah direktori.

```

``````

try (ArjArchive archive = new ArjArchive("archive.arj")) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry. See [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\#extract-java.io.OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### ArjArchive(String path, ArjLoadOptions loadOptions) {#ArjArchive-java.lang.String-com.aspose.zip.ArjLoadOptions-}
```
public ArjArchive(String path, ArjLoadOptions loadOptions)
```


Initializes a new instance of the [ArjArchive](../../com.aspose.zip/arjarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (ArjArchive archive = new ArjArchive("archive.arj")) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

Konstruktor ini tidak membuka (unpack) entri apa pun. Lihat metode [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\\#extract-java.io.OutputStream-) untuk mendekompresi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | java.lang.String | jalur ke file arsip |
| loadOptions | [ArjLoadOptions](../../com.aspose.zip/arjloadoptions) | Opsi untuk memuat arsip yang ada. |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Mengekstrak semua entri ke direktori yang ditentukan.

Contoh berikut menunjukkan cara mengekstrak semua entri ke sebuah direktori:

```

``````

try (ArjArchive archive = new ArjArchive(new FileInputStream("archive.arj"))) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the directory to extract the entries to |

### getCommentary() {#getCommentary--}
```
public final String getCommentary()
```


Gets the commentary.

**Returns:**
java.lang.String - the commentary.
### getEntries() {#getEntries--}
```
public final List<ArjEntryPlain> getEntries()
```


Gets entries of [ArjEntryPlain](../../com.aspose.zip/arjentryplain) type constituting the ARJ archive.

**Returns:**
java.util.List&lt;com.aspose.zip.ArjEntryPlain&gt; - entries of [ArjEntryPlain](../../com.aspose.zip/arjentryplain) type constituting the ARJ archive.
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
### getName() {#getName--}
```
public final String getName()
```


Gets the original name.

**Returns:**
java.lang.String - the original name.
