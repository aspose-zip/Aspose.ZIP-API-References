---
title: "LhaArchiveEntry"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Mewakili satu berkas dalam arsip Lha."
type: docs
weight: 76
url: /id/java/com.aspose.zip/lhaarchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class LhaArchiveEntry implements IArchiveFileEntry
```

Mewakili satu berkas dalam arsip Lha.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [extract(File file)](#extract-java.io.File-) | Mengekstrak entri arsip Lha ke sebuah file. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Mengekstrak entri ke aliran yang disediakan. |
| [extract(String path)](#extract-java.lang.String-) | Mengekstrak entri arsip Lha ke sistem file berdasarkan path. |
| [getLastModified()](#getLastModified--) | Mendapatkan waktu terakhir dimodifikasi dari entri. |
| [getLength()](#getLength--) | Mendapatkan panjang entri dalam byte. |
| [getModificationTime()](#getModificationTime--) | Mendapatkan waktu terakhir dimodifikasi dari entri. |
| [getName()](#getName--) | Mendapatkan nama entri. |
| [getPath()](#getPath--) | Mendapatkan path lengkap ke entri. |
| [isDirectory()](#isDirectory--) | Mendapatkan nilai yang menunjukkan apakah entri ini adalah direktori. |
### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Mengekstrak entri arsip Lha ke sebuah file.

```

``````

try (FileInputStream lhaFile = new FileInputStream(\"archive.lha\")) {
try (LhaArchive archive = new LhaArchive(lhaFile)) {
archive.getEntries().get(0).extract(new File(\"extracted.bin\"));
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | File for storing decompressed data.

Does nothing for directory entry |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts the entry to the stream provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts Lha archive entry to a filesystem by path.

```

``````

     try (FileInputStream lhaFile = new FileInputStream("archive.lha")) {
         try (LhaArchive archive = new LhaArchive(lhaFile)) {
             archive.getEntries().get(0).extract("extracted.bin");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | java.lang.String | path ke file yang akan menyimpan data terdekompresi |

**Returns:**
java.io.File - instance java.io.File yang berisi data yang diekstrak
### getLastModified() {#getLastModified--}
```
public final Date getLastModified()
```


Mendapatkan waktu terakhir dimodifikasi dari entri.

**Returns:**
java.util.Date - waktu terakhir dimodifikasi dari entri
### getLength() {#getLength--}
```
public final Long getLength()
```


Mendapatkan panjang entri dalam byte.

**Returns:**
java.lang.Long - panjang entri dalam byte
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Mendapatkan waktu terakhir dimodifikasi dari entri.

**Returns:**
java.util.Date - waktu terakhir dimodifikasi dari entri
### getName() {#getName--}
```
public final String getName()
```


Mendapatkan nama entri.

Arsip hanya untuk kompresi, seperti gzip, bzip2, lzip, lzma, xz, z memiliki nama \"File.bin\" kecuali nama lain dapat ditemukan di header.

**Returns:**
java.lang.String - nama entri
### getPath() {#getPath--}
```
public final String getPath()
```


Mendapatkan path lengkap ke entri.

**Returns:**
java.lang.String - path lengkap ke entri
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Mendapatkan nilai yang menunjukkan apakah entri ini adalah direktori.

**Returns:**
boolean - nilai yang menunjukkan apakah entri ini adalah direktori.
