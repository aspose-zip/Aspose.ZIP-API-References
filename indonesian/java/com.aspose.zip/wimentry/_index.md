---
title: "WimEntry"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Mewakili satu file atau direktori dalam gambar wim."
type: docs
weight: 132
url: /id/java/com.aspose.zip/wimentry/
---

**Inheritance:**
java.lang.Object
```
public abstract class WimEntry
```

Mewakili satu file atau direktori dalam gambar wim.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getAlternateDataStreams()](#getAlternateDataStreams--) | Mendapatkan nama-nama aliran data alternatif untuk file atau direktori. |
| [getArchive()](#getArchive--) | Mendapatkan arsip tempat entri tersebut berada. |
| [getChangeTime()](#getChangeTime--) | Mendapatkan waktu terakhir file atau direktori diubah. |
| [getCreationTime()](#getCreationTime--) | Mendapatkan waktu pembuatan file atau direktori. |
| [getFileAttributes()](#getFileAttributes--) | Mendapatkan atribut file atau direktori. |
| [getFullPath()](#getFullPath--) | Mendapatkan jalur lengkap entri dalam citra. |
| [getHardLink()](#getHardLink--) | Mendapatkan ID hardlink file atau direktori. |
| [getImage()](#getImage--) | Mendapatkan citra tempat entri berada. |
| [getLastAccessTime()](#getLastAccessTime--) | Mendapatkan waktu akses terakhir file atau direktori. |
| [getLastWriteTime()](#getLastWriteTime--) | Mendapatkan waktu modifikasi file atau direktori. |
| [getModificationTime()](#getModificationTime--) | Mendapatkan waktu modifikasi file atau direktori. |
| [getName()](#getName--) | Mendapatkan nama entri dalam citra. |
| [getParent()](#getParent--) | Mendapatkan direktori induk tempat entri berada. |
| [getShortName()](#getShortName--) | Mendapatkan nama pendek entri dalam citra. |
| [hasHardLinks()](#hasHardLinks--) | Mendapatkan apakah file atau direktori dikenal dengan nama lain. |
| [isDirectory()](#isDirectory--) | Mendapatkan nilai yang menunjukkan apakah entri mewakili sebuah direktori. |
| [toString()](#toString--) | Mengembalikan representasi string dari instance kelas [WimEntry](../../com.aspose.zip/wimentry). |
### getAlternateDataStreams() {#getAlternateDataStreams--}
```
public final String[] getAlternateDataStreams()
```


Mendapatkan nama-nama aliran data alternatif untuk file atau direktori.

**Returns:**
java.lang.String[] - nama-nama aliran data alternatif untuk file atau direktori
### getArchive() {#getArchive--}
```
public final WimArchive getArchive()
```


Mendapatkan arsip tempat entri tersebut berada.

**Returns:**
[WimArchive](../../com.aspose.zip/wimarchive) - the archive the entry belongs to
### getChangeTime() {#getChangeTime--}
```
public final Date getChangeTime()
```


Mendapatkan waktu terakhir file atau direktori diubah.

**Returns:**
java.util.Date - waktu terakhir file atau direktori diubah
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


Mendapatkan waktu pembuatan file atau direktori.

**Returns:**
java.util.Date - waktu pembuatan file atau direktori
### getFileAttributes() {#getFileAttributes--}
```
public final int getFileAttributes()
```


Mendapatkan atribut file atau direktori.

**Returns:**
int - atribut file atau direktori
### getFullPath() {#getFullPath--}
```
public final String getFullPath()
```


Mendapatkan jalur lengkap entri dalam citra.

**Returns:**
java.lang.String - jalur lengkap entri dalam gambar
### getHardLink() {#getHardLink--}
```
public final long getHardLink()
```


Mendapatkan ID hardlink file atau direktori.

**Returns:**
long - id hardlink file atau direktori
### getImage() {#getImage--}
```
public final WimImage getImage()
```


Mendapatkan citra tempat entri berada.

**Returns:**
[WimImage](../../com.aspose.zip/wimimage) - the image the entry belongs to
### getLastAccessTime() {#getLastAccessTime--}
```
public final Date getLastAccessTime()
```


Mendapatkan waktu akses terakhir file atau direktori.

**Returns:**
java.util.Date - waktu akses terakhir file atau direktori
### getLastWriteTime() {#getLastWriteTime--}
```
public final Date getLastWriteTime()
```


Mendapatkan waktu modifikasi file atau direktori.

**Returns:**
java.util.Date - waktu modifikasi file atau direktori
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Mendapatkan waktu modifikasi file atau direktori.

**Returns:**
java.util.Date - waktu modifikasi file atau direktori
### getName() {#getName--}
```
public final String getName()
```


Mendapatkan nama entri dalam citra.

**Returns:**
java.lang.String - nama entri dalam gambar
### getParent() {#getParent--}
```
public final WimDirectoryEntry getParent()
```


Mendapatkan direktori induk tempat entri berada.

**Returns:**
[WimDirectoryEntry](../../com.aspose.zip/wimdirectoryentry) - the parent directory the entry belongs to
### getShortName() {#getShortName--}
```
public final String getShortName()
```


Mendapatkan nama pendek entri dalam citra.

**Returns:**
java.lang.String - nama pendek entri dalam gambar
### hasHardLinks() {#hasHardLinks--}
```
public final boolean hasHardLinks()
```


Mendapatkan apakah file atau direktori dikenal dengan nama lain.

**Returns:**
boolean - apakah file atau direktori dikenal dengan nama lain
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Mendapatkan nilai yang menunjukkan apakah entri mewakili sebuah direktori.

**Returns:**
boolean - nilai yang menunjukkan apakah entri merupakan direktori
### toString() {#toString--}
```
public String toString()
```


Mengembalikan representasi string dari instance kelas [WimEntry](../../com.aspose.zip/wimentry).

**Returns:**
java.lang.String - representasi string dari objek ini
