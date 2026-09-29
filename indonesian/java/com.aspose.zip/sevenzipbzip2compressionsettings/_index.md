---
title: "SevenZipBZip2CompressionSettings"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Pengaturan untuk metode kompresi BZip2 dalam arsip 7z."
type: docs
weight: 109
url: /id/java/com.aspose.zip/sevenzipbzip2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public class SevenZipBZip2CompressionSettings extends SevenZipCompressionSettings
```

Pengaturan untuk metode kompresi BZip2 dalam arsip 7z.

Bzip2 mengompresi file menggunakan algoritma kompresi teks penyortiran blok Burrows-Wheeler, dan pengkodean Huffman.

Lihat selengkapnya: [Bzip2][]


[Bzip2]: https://en.wikipedia.org/wiki/Bzip2
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [SevenZipBZip2CompressionSettings(int blockSize)](#SevenZipBZip2CompressionSettings-int-) | Menginisialisasi instance baru dari kelas [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings). |
| [SevenZipBZip2CompressionSettings()](#SevenZipBZip2CompressionSettings--) | Menginisialisasi instance baru dari kelas [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings) dengan ukuran blok default, setara dengan 9 ratus kilobyte. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Ukuran blok dalam ratus kilobyte. |
| [getMethod()](#getMethod--) | Mendapatkan metode kompresi atau dekompresi. |
### SevenZipBZip2CompressionSettings(int blockSize) {#SevenZipBZip2CompressionSettings-int-}
```
public SevenZipBZip2CompressionSettings(int blockSize)
```


Menginisialisasi instance baru dari kelas [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| blockSize | int | ukuran blok dalam ratus kilobyte |

### SevenZipBZip2CompressionSettings() {#SevenZipBZip2CompressionSettings--}
```
public SevenZipBZip2CompressionSettings()
```


Menginisialisasi instance baru dari kelas [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings) dengan ukuran blok default, setara dengan 9 ratus kilobyte.

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


Ukuran blok dalam ratus kilobyte.

**Returns:**
int - ukuran blok dalam ratus kilobyte
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


Mendapatkan metode kompresi atau dekompresi.

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method
