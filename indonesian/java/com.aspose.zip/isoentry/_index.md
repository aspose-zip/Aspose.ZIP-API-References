---
title: "IsoEntry"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Mewakili sebuah file entri atau direktori dalam arsip ISO."
type: docs
weight: 72
url: /id/java/com.aspose.zip/isoentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class IsoEntry implements IArchiveFileEntry
```

Mewakili entri (berkas atau direktori) dalam arsip ISO.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Mengekstrak entri ke aliran yang disediakan. |
| [extract(String path)](#extract-java.lang.String-) | Mengekstrak entri ke sistem file menggunakan jalur yang disediakan. |
| [getLength()](#getLength--) | Mendapatkan panjang entri. |
| [getModificationTime()](#getModificationTime--) | Mendapatkan tanggal dan waktu terakhir dimodifikasi. |
| [getName()](#getName--) | Mendapatkan nama entri. |
| [isDirectory()](#isDirectory--) | Mendapatkan nilai yang menunjukkan apakah entri adalah direktori. |
| [toString()](#toString--) | Mengembalikan string yang mewakili entri saat ini. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public void extract(OutputStream destination)
```


Mengekstrak entri ke aliran yang disediakan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| tujuan | java.io.OutputStream | stream tujuan |

### extract(String path) {#extract-java.lang.String-}
```
public File extract(String path)
```


Mengekstrak entri ke sistem file menggunakan jalur yang disediakan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | java.lang.String | jalur ke file tujuan. Jika file sudah ada, akan ditimpa |

**Returns:**
java.io.File - instance java.io.File yang berisi data yang diekstrak
### getLength() {#getLength--}
```
public Long getLength()
```


Mendapatkan panjang entri.

**Returns:**
java.lang.Long - panjang entri
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Mendapatkan tanggal dan waktu terakhir dimodifikasi.

**Returns:**
java.util.Date - tanggal dan waktu terakhir dimodifikasi
### getName() {#getName--}
```
public final String getName()
```


Mendapatkan nama entri.

**Returns:**
java.lang.String - nama entri
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Mendapatkan nilai yang menunjukkan apakah entri adalah direktori.

**Returns:**
boolean - nilai yang menunjukkan apakah entri merupakan direktori
### toString() {#toString--}
```
public String toString()
```


Mengembalikan string yang mewakili entri saat ini.

**Returns:**
java.lang.String - nama entri
