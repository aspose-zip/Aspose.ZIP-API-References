---
title: "TarEntry"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Mewakili satu file dalam arsip tar."
type: docs
weight: 126
url: /id/java/com.aspose.zip/tarentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class TarEntry implements IArchiveFileEntry
```

Mewakili satu file dalam arsip tar.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Mengekstrak entri ke aliran yang disediakan. |
| [extract(String path)](#extract-java.lang.String-) | Mengekstrak entri ke sistem file menggunakan jalur yang disediakan. |
| [getLength()](#getLength--) | Mendapatkan panjang entri dalam byte. |
| [getModificationTime()](#getModificationTime--) | Mendapatkan waktu modifikasi file atau direktori. |
| [getName()](#getName--) | Mendapatkan nama entri di dalam arsip. |
| [getUncompressedSize()](#getUncompressedSize--) | Mendapatkan ukuran file asli. |
| [isDirectory()](#isDirectory--) | Mendapatkan nilai yang menunjukkan apakah entri mewakili sebuah direktori. |
| [open()](#open--) | Membuka entri untuk ekstraksi dan menyediakan aliran dengan konten entri. |
| [setName(String value)](#setName-java.lang.String-) | Mengatur nama entri di dalam arsip. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Mengekstrak entri ke aliran yang disediakan.

Ekstrak sebuah entri dari arsip tar.

```

``````

try (TarArchive archive = new TarArchive("archive.tar")) {
archive.getEntries().get_Item(0).extract(httpResponseStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | Destination stream. Must be writable. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the entry to the filesystem by the path provided.

```

``````

     try (TarArchive archive = new TarArchive("archive.tar")) {
         archive.getEntries().get_Item(0).extract("data.bin");
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | java.lang.String | jalur ke file tujuan. Jika file sudah ada, akan ditimpa. |

**Returns:**
java.io.File - informasi file dari file yang diekstrak
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


Mendapatkan waktu modifikasi file atau direktori.

**Returns:**
java.util.Date - waktu modifikasi file atau direktori.
### getName() {#getName--}
```
public final String getName()
```


Mendapatkan nama entri di dalam arsip.

**Returns:**
java.lang.String - nama entri di dalam arsip
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Mendapatkan ukuran file asli.

Memiliki nilai yang sama dengan `Length`([getLength](../../com.aspose.zip/tarentry\#getLength--))

**Returns:**
long - ukuran file asli.
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Mendapatkan nilai yang menunjukkan apakah entri mewakili sebuah direktori.

**Returns:**
boolean - nilai yang menunjukkan apakah entri merupakan direktori
### open() {#open--}
```
public final InputStream open()
```


Membuka entri untuk ekstraksi dan menyediakan aliran dengan konten entri.


Penggunaan:

```

``````

InputStream decompressed = entry.open();
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
fileStream.write(buffer, 0, bytesRead);
}
 
```

Read from the stream to get the original content of the file. See examples section.

**Returns:**
java.io.InputStream - the stream that represents the contents of the entry
### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Sets the name of the entry within the archive.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the name of the entry within the archive |

