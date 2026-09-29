---
title: "IArchiveFileEntry"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Antarmuka ini mewakili entri berkas arsip."
type: docs
weight: 162
url: /id/java/com.aspose.zip/iarchivefileentry/
---
```
public interface IArchiveFileEntry
```

Antarmuka ini mewakili entri berkas arsip.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Mengekstrak entri ke aliran yang disediakan. |
| [extract(String path)](#extract-java.lang.String-) | Mengekstrak entri ke sistem file menggunakan jalur yang disediakan. |
| [getLength()](#getLength--) | Mendapatkan panjang entri dalam byte. |
| [getName()](#getName--) | Mendapatkan nama entri. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public abstract void extract(OutputStream destination)
```


Mengekstrak entri ke aliran yang disediakan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| tujuan | java.io.OutputStream | stream tujuan. Harus dapat ditulis |

### extract(String path) {#extract-java.lang.String-}
```
public abstract File extract(String path)
```


Mengekstrak entri ke sistem file menggunakan jalur yang disediakan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | java.lang.String | jalur ke file tujuan. Jika file sudah ada, akan ditimpa. |

**Returns:**
java.io.File - instance java.io.File yang berisi data yang diekstrak
### getLength() {#getLength--}
```
public abstract Long getLength()
```


Mendapatkan panjang entri dalam byte.

**Returns:**
java.lang.Long - panjang entri dalam byte
### getName() {#getName--}
```
public abstract String getName()
```


Mendapatkan nama entri.

Arsip hanya untuk kompresi, seperti gzip, bzip2, lzip, lzma, xz, z memiliki nama \"File.bin\" kecuali nama lain dapat ditemukan di header.

**Returns:**
java.lang.String - nama entri
