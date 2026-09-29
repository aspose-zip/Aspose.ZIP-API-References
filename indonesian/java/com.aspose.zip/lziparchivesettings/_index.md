---
title: "LzipArchiveSettings"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Kelas ini berisi pengaturan untuk arsip lzip tertentu."
type: docs
weight: 84
url: /id/java/com.aspose.zip/lziparchivesettings/
---

**Inheritance:**
java.lang.Object
```
public class LzipArchiveSettings
```

Kelas ini berisi pengaturan untuk arsip lzip tertentu.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [LzipArchiveSettings(int dictionarySize)](#LzipArchiveSettings-int-) | Menginisialisasi sebuah instance baru dari [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) dengan ukuran kamus tertentu. |
| [LzipArchiveSettings(int dictionarySize, int maxMemberSize)](#LzipArchiveSettings-int-int-) | Menginisialisasi sebuah instance baru dari [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) dengan ukuran kamus tertentu. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getCompressionThreads()](#getCompressionThreads--) | Mendapatkan jumlah thread kompresi. |
| [getDictionarySize()](#getDictionarySize--) | Mendapatkan ukuran kamus yang digunakan oleh kompresi LZMA. |
| [getFastSpeed()](#getFastSpeed--) | Mendapatkan instance dari kelas [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) dengan ukuran kamus sebesar 1 megabyte dalam filter LZMA. |
| [getFastestSpeed()](#getFastestSpeed--) | Mendapatkan instance dari kelas [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) dengan ukuran kamus sebesar 65536 byte dalam filter LZMA. |
| [getHighCompression()](#getHighCompression--) | Mendapatkan instance dari kelas [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) dengan ukuran kamus sebesar 32 megabyte dalam filter LZMA. |
| [getMaxMemberSize()](#getMaxMemberSize--) | Mendapatkan ukuran maksimum satu anggota dalam arsip lzip yang ditampilkan dalam byte. |
| [getMaximumCompression()](#getMaximumCompression--) | Mendapatkan instance dari kelas [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) dengan ukuran kamus sebesar 64 megabyte dalam filter LZMA. |
| [getNormal()](#getNormal--) | Mendapatkan instance dari kelas [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) dengan ukuran kamus sebesar 16 megabyte dalam filter LZMA. |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | Mengatur jumlah thread kompresi. |
### LzipArchiveSettings(int dictionarySize) {#LzipArchiveSettings-int-}
```
public LzipArchiveSettings(int dictionarySize)
```


Menginisialisasi sebuah instance baru dari [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) dengan ukuran kamus tertentu.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| dictionarySize | int | ukuran kamus untuk kompresi LZMA dalam byte |

### LzipArchiveSettings(int dictionarySize, int maxMemberSize) {#LzipArchiveSettings-int-int-}
```
public LzipArchiveSettings(int dictionarySize, int maxMemberSize)
```


Menginisialisasi sebuah instance baru dari [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) dengan ukuran kamus tertentu.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| dictionarySize | int | ukuran kamus untuk kompresi LZMA dalam byte |
| maxMemberSize | int | Ukuran maksimum satu anggota dalam arsip lzip yang ditampilkan dalam byte. Nilai default adalah 60 MB. |

### getCompressionThreads() {#getCompressionThreads--}
```
public final int getCompressionThreads()
```


Mendapatkan jumlah utas kompresi. Jika nilai lebih besar dari 1, kompresi multithreading akan digunakan.

**Returns:**
int - jumlah utas kompresi
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


Mendapatkan ukuran kamus yang digunakan oleh kompresi LZMA.

**Returns:**
int - ukuran kamus yang digunakan oleh kompresi LZMA
### getFastSpeed() {#getFastSpeed--}
```
public static LzipArchiveSettings getFastSpeed()
```


Mendapatkan instance dari kelas [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) dengan ukuran kamus sebesar 1 megabyte dalam filter LZMA.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 1 megabyte in LZMA filter
### getFastestSpeed() {#getFastestSpeed--}
```
public static LzipArchiveSettings getFastestSpeed()
```


Mendapatkan instance dari kelas [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) dengan ukuran kamus sebesar 65536 byte dalam filter LZMA.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 65536 bytes in LZMA filter
### getHighCompression() {#getHighCompression--}
```
public static LzipArchiveSettings getHighCompression()
```


Mendapatkan instance dari kelas [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) dengan ukuran kamus sebesar 32 megabyte dalam filter LZMA.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 32 megabytes in LZMA filter
### getMaxMemberSize() {#getMaxMemberSize--}
```
public final long getMaxMemberSize()
```


Mendapatkan ukuran maksimum satu anggota dalam arsip lzip yang ditampilkan dalam byte.

**Returns:**
long - ukuran maksimum satu anggota dalam arsip lzip yang ditampilkan dalam byte
### getMaximumCompression() {#getMaximumCompression--}
```
public static LzipArchiveSettings getMaximumCompression()
```


Mendapatkan instance dari kelas [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) dengan ukuran kamus sebesar 64 megabyte dalam filter LZMA.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 64 megabytes in LZMA filter
### getNormal() {#getNormal--}
```
public static LzipArchiveSettings getNormal()
```


Mendapatkan instance dari kelas [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) dengan ukuran kamus sebesar 16 megabyte dalam filter LZMA.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 16 megabytes in LZMA filter
### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


Mengatur jumlah thread kompresi. Jika nilai lebih besar dari 1, kompresi multithread akan digunakan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | jumlah thread kompresi |

