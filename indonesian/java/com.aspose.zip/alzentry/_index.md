---
title: "AlzEntry"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Mewakili entri file dalam arsip ALZ bersama dengan metadata-nya."
type: docs
weight: 13
url: /id/java/com.aspose.zip/alzentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class AlzEntry implements IArchiveFileEntry
```

Mewakili entri file dalam arsip ALZ bersama dengan metadata-nya.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Mengekstrak entri ke aliran yang dapat ditulis. |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | Mengekstrak entri ke aliran yang dapat ditulis menggunakan kata sandi opsional. |
| [extract(String path)](#extract-java.lang.String-) | Mengekstrak entri ke file yang ditentukan. |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | Mengekstrak entri ke file yang ditentukan menggunakan kata sandi opsional. |
| [getCompressedSize()](#getCompressedSize--) | Mendapatkan ukuran terkompresi data entri dalam byte. |
| [getLength()](#getLength--) | Mendapatkan panjang tidak terkompresi entri ini. |
| [getName()](#getName--) | Mendapatkan nama entri yang disimpan dalam arsip. |
| [getUncompressedSize()](#getUncompressedSize--) | Mendapatkan ukuran tidak terkompresi data entri dalam byte. |
| [isDirectory()](#isDirectory--) | Mendapatkan apakah entri ini mewakili sebuah direktori. |
| [open()](#open--) | Membuka entri dan menyediakan aliran yang berisi data yang telah didekompresi. |
| [open(String password)](#open-java.lang.String-) | Membuka entri dan menyediakan aliran yang berisi data yang telah didekompresi. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Mengekstrak entri ke aliran yang dapat ditulis.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| tujuan | java.io.OutputStream | stream tujuan |

### extract(OutputStream destination, String password) {#extract-java.io.OutputStream-java.lang.String-}
```
public final void extract(OutputStream destination, String password)
```


Mengekstrak entri ke aliran yang dapat ditulis menggunakan kata sandi opsional.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| tujuan | java.io.OutputStream | stream tujuan |
| password | java.lang.String | kata sandi opsional untuk entri ini |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Mengekstrak entri ke file yang ditentukan. File yang ada akan ditimpa.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | java.lang.String | jalur file tujuan |

**Returns:**
java.io.File - file yang diekstrak
### extract(String path, String password) {#extract-java.lang.String-java.lang.String-}
```
public final File extract(String path, String password)
```


Mengekstrak entri ke file yang ditentukan menggunakan kata sandi opsional.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | java.lang.String | jalur file tujuan |
| password | java.lang.String | kata sandi opsional untuk entri ini |

**Returns:**
java.io.File - file yang diekstrak
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Mendapatkan ukuran terkompresi data entri dalam byte.

**Returns:**
long - ukuran terkompres dalam byte
### getLength() {#getLength--}
```
public final Long getLength()
```


Mendapatkan panjang tidak terkompresi entri ini.

**Returns:**
java.lang.Long - panjang tidak terkompres dalam byte
### getName() {#getName--}
```
public final String getName()
```


Mendapatkan nama entri yang disimpan dalam arsip.

**Returns:**
java.lang.String - nama entri
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Mendapatkan ukuran tidak terkompresi data entri dalam byte.

**Returns:**
long - ukuran tidak terkompres dalam byte
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Mendapatkan apakah entri ini mewakili sebuah direktori.

**Returns:**
boolean - `true` untuk entri direktori
### open() {#open--}
```
public final InputStream open()
```


Membuka entri dan menyediakan aliran yang berisi data yang telah didekompresi.

**Returns:**
java.io.InputStream - aliran yang berisi data entri yang didekompresi
### open(String password) {#open-java.lang.String-}
```
public final InputStream open(String password)
```


Membuka entri dan menyediakan aliran yang berisi data yang telah didekompresi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| password | java.lang.String | kata sandi opsional untuk entri ini |

**Returns:**
java.io.InputStream - aliran yang berisi data entri yang didekompresi
