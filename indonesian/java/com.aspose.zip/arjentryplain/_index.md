---
title: "ArjEntryPlain"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Mewakili satu file dalam arsip ARJ."
type: docs
weight: 38
url: /id/java/com.aspose.zip/arjentryplain/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class ArjEntryPlain implements IArchiveFileEntry
```

Mewakili satu file dalam arsip ARJ.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [extract(File file)](#extract-java.io.File-) | Mengekstrak entri arsip ARJ ke sebuah file. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Mengekstrak entri ke aliran yang disediakan. |
| [extract(String path)](#extract-java.lang.String-) | Mengekstrak entri ke sistem file menggunakan jalur yang disediakan. |
| [getCompressedSize()](#getCompressedSize--) | Mendapatkan ukuran file terkompresi. |
| [getLength()](#getLength--) | Mendapatkan panjang entri dalam byte. |
| [getName()](#getName--) | Mendapatkan nama entri dalam arsip. |
| [getUncompressedSize()](#getUncompressedSize--) | Mendapatkan ukuran file asli. |
### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Mengekstrak entri arsip ARJ ke sebuah file.

```

``````

try (FileInputStream arjFile = new FileInputStream("sourceFileName")) {
try (ArjArchive archive = new ArjArchive(arjFile)) {
archive.getEntries().get(0).extract(new File(\"extracted.bin\"));
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | java.io.File for storing decompressed data |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts the entry to the stream provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | Destination stream. Must be writable. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the entry to the filesystem by the path provided.

Extract two entries of rar archive.

```

``````

     try (FileInputStream arjFile = new FileInputStream("archive.arj")) {
         try (ArjArchive archive = new ArjArchive(arjFile)) {
             archive.getEntries().get(0).extract("first.bin");
             archive.getEntries().get(1).extract("second.bin");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | java.lang.String | jalur ke file tujuan. Jika file sudah ada, akan ditimpa. |

**Returns:**
java.io.File - informasi berkas dari berkas yang disusun
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Mendapatkan ukuran file terkompresi.

**Returns:**
long - ukuran file terkompresi
### getLength() {#getLength--}
```
public final Long getLength()
```


Mendapatkan panjang entri dalam byte.

**Returns:**
java.lang.Long - panjang entri dalam byte
### getName() {#getName--}
```
public final String getName()
```


Mendapatkan nama entri dalam arsip.

**Returns:**
java.lang.String - nama entri di dalam arsip
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Mendapatkan ukuran file asli.

**Returns:**
long - ukuran berkas asli
