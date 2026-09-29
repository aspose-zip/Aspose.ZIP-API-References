---
title: "SevenZipLZMA2CompressionSettings"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Pengaturan untuk metode kompresi LZMA2 dalam arsip 7z."
type: docs
weight: 114
url: /id/java/com.aspose.zip/sevenziplzma2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public class SevenZipLZMA2CompressionSettings extends SevenZipCompressionSettings
```

Pengaturan untuk metode kompresi LZMA2 dalam arsip 7z.

LZMA2 mendukung beberapa putaran data LZMA terkompresi dan data tidak terkompresi.

Lihat selengkapnya: [Lempel\u2013Ziv\u2013Markov\_chain\_algorithm][Lempel_u2013Ziv_u2013Markov_chain_algorithm]


[Lempel_u2013Ziv_u2013Markov_chain_algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [SevenZipLZMA2CompressionSettings()](#SevenZipLZMA2CompressionSettings--) | Membuat instance pengaturan untuk metode kompresi LZMA2 dalam arsip 7z. |
| [SevenZipLZMA2CompressionSettings(int dictionarySize)](#SevenZipLZMA2CompressionSettings-int-) | Membuat instance pengaturan untuk metode kompresi LZMA2 dalam arsip 7z. |
| [SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes)](#SevenZipLZMA2CompressionSettings-int-int-) | Membuat instance pengaturan untuk metode kompresi LZMA2 dalam arsip 7z. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getCompressionThreads()](#getCompressionThreads--) | Mendapatkan jumlah thread kompresi. |
| [getDictionarySize()](#getDictionarySize--) | Ukuran kamus (buffer riwayat) menunjukkan berapa byte data tidak terkompresi yang baru saja diproses yang disimpan dalam memori. |
| [getFastBytes()](#getFastBytes--) | Mendapatkan nomor kontrol byte cepat yang digunakan oleh kompresor LZMA2. |
| [getMethod()](#getMethod--) | Mendapatkan metode kompresi atau dekompresi. |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | Mengatur jumlah thread kompresi. |
### SevenZipLZMA2CompressionSettings() {#SevenZipLZMA2CompressionSettings--}
```
public SevenZipLZMA2CompressionSettings()
```


Membuat instance pengaturan untuk metode kompresi LZMA2 dalam arsip 7z.

### SevenZipLZMA2CompressionSettings(int dictionarySize) {#SevenZipLZMA2CompressionSettings-int-}
```
public SevenZipLZMA2CompressionSettings(int dictionarySize)
```


Membuat instance pengaturan untuk metode kompresi LZMA2 dalam arsip 7z.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | dictionarySize | int | ukuran buffer riwayat, harus antara 4096 dan 1073741824. |

Semakin besar kamus, biasanya rasio kompresi lebih baik - tetapi kamus yang lebih besar daripada data tidak terkompresi merupakan pemborosan RAM. |

### SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes) {#SevenZipLZMA2CompressionSettings-int-int-}
```
public SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes)
```


Membuat instance pengaturan untuk metode kompresi LZMA2 dalam arsip 7z.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | dictionarySize | int | ukuran buffer riwayat, harus antara 4096 dan 1073741824. |

Semakin besar kamus, biasanya rasio kompresi lebih baik - tetapi kamus yang lebih besar daripada data tidak terkompresi merupakan pemborosan RAM. |
| fastBytes | int | mengontrol jumlah byte cepat yang digunakan oleh kompresor LZMA2. Jumlah byte cepat yang lebih besar dapat memberikan rasio kompresi yang lebih baik dengan mengorbankan kecepatan kompresi. |

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


Ukuran kamus (buffer riwayat) menunjukkan berapa byte data tidak terkompresi yang baru saja diproses yang disimpan dalam memori.

**Returns:**
int - ukuran kamus (buffer riwayat)
### getFastBytes() {#getFastBytes--}
```
public final int getFastBytes()
```


Mendapatkan nomor kontrol byte cepat yang digunakan oleh kompresor LZMA2.

**Returns:**
int - nomor kontrol byte cepat yang digunakan oleh kompresor LZMA2
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


Mendapatkan metode kompresi atau dekompresi.

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method.
### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


Mengatur jumlah thread kompresi. Jika nilai lebih besar dari 1, kompresi multithread akan digunakan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | int | jumlah thread kompresi. |

Jangan atur angka ini lebih dari inti CPU. |

