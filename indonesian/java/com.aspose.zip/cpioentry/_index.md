---
title: "CpioEntry"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Mewakili satu file dalam arsip cpio."
type: docs
weight: 58
url: /id/java/com.aspose.zip/cpioentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public final class CpioEntry implements IArchiveFileEntry
```

Mewakili satu file dalam arsip cpio.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Mengekstrak entri ke aliran yang disediakan. |
| [extract(String path)](#extract-java.lang.String-) | Mengekstrak entri ke sistem file menggunakan jalur yang disediakan. |
| [getLastWriteTimeUtc()](#getLastWriteTimeUtc--) | Mendapatkan waktu penulisan terakhir. |
| [getLength()](#getLength--) | Mendapatkan panjang entri dalam byte. |
| [getName()](#getName--) | Mendapatkan nama entri di dalam arsip. |
| [getParent()](#getParent--) | Mendapatkan arsip tempat entri tersebut berada. |
| [isDirectory()](#isDirectory--) | Mendapatkan nilai yang menunjukkan apakah entri mewakili sebuah direktori. |
| [open()](#open--) | Membuka entri untuk ekstraksi dan menyediakan aliran dengan konten entri. |
| [toString()](#toString--) | Mengembalikan representasi string dari instance kelas [CpioEntry](../../com.aspose.zip/cpioentry). |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Mengekstrak entri ke aliran yang disediakan.

Ekstrak sebuah entri dari arsip cpio.

```

``````

try (CpioArchive archive = new CpioArchive("archive.cpio")) {
archive.getEntries().get(0).extract(httpResponseStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream. Must be writable |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the entry to the filesystem by the path provided.

```

``````

     try (CpioArchive archive = new CpioArchive("archive.cpio")) {
         archive.getEntries().get(0).extract("data.bin");
     }
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | java.lang.String | jalur ke file tujuan. Jika file sudah ada, akan ditimpa. |

**Returns:**
java.io.File - informasi file dari file yang diekstrak
### getLastWriteTimeUtc() {#getLastWriteTimeUtc--}
```
public final Date getLastWriteTimeUtc()
```


Mendapatkan waktu penulisan terakhir.

**Returns:**
java.util.Date - waktu penulisan terakhir
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


Mendapatkan nama entri di dalam arsip.

**Returns:**
java.lang.String - nama entri di dalam arsip
### getParent() {#getParent--}
```
public final CpioArchive getParent()
```


Mendapatkan arsip tempat entri tersebut berada.

**Returns:**
[CpioArchive](../../com.aspose.zip/cpioarchive) - the archive the entry belongs to
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Mendapatkan nilai yang menunjukkan apakah entri mewakili sebuah direktori.

**Returns:**
boolean - nilai yang menunjukkan apakah entri merupakan direktori.
### open() {#open--}
```
public final InputStream open()
```


Membuka entri untuk ekstraksi dan menyediakan aliran dengan konten entri.

Penggunaan:

```

``````

CpioArchive archive = new CpioArchive("archive.cpio");
CpioEntry entry = archive.getEntries().get(0);
try (FileOutputStream fileStream = new FileOutputStream("data.bin")) {
try (InputStream decompressed = entry.open()) {
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
fileStream.write(buffer, 0, bytesRead);
}
}
} catch (IOException ex) {
}
 
```

Read from the stream to get the original content of a file. See examples section.

**Returns:**
java.io.InputStream - the stream that represents the contents of the entry
### toString() {#toString--}
```
public String toString()
```


Returns string representation of the instance of the [CpioEntry](../../com.aspose.zip/cpioentry) class.

**Returns:**
java.lang.String - string representation of this object.
