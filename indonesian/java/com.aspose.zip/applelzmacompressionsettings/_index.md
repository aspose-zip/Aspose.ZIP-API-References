---
title: "AppleLzmaCompressionSettings"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Pengaturan untuk kompresi LZMA dalam file Apple Archive .aar."
type: docs
weight: 23
url: /id/java/com.aspose.zip/applelzmacompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings)
```
public class AppleLzmaCompressionSettings extends AppleCompressionSettings
```

Pengaturan untuk kompresi LZMA dalam file Apple Archive (.aar).
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [AppleLzmaCompressionSettings(int blockSize)](#AppleLzmaCompressionSettings-int-) | Menginisialisasi sebuah instance baru dari kelas [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings). |
| [AppleLzmaCompressionSettings(int blockSize, int dictionarySize)](#AppleLzmaCompressionSettings-int-int-) | Menginisialisasi sebuah instance baru dari kelas [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings). |
| [AppleLzmaCompressionSettings(int blockSize, int dictionarySize, int fastBytes)](#AppleLzmaCompressionSettings-int-int-int-) | Menginisialisasi sebuah instance baru dari kelas [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings). |
| [AppleLzmaCompressionSettings()](#AppleLzmaCompressionSettings--) | Menginisialisasi sebuah instance baru dari kelas [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) dengan parameter default. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Mendapatkan ukuran setiap blok data sebelum kompresi. |
| [getDictionarySize()](#getDictionarySize--) | Mendapatkan ukuran kamus yang digunakan untuk kompresi. |
| [getFastBytes()](#getFastBytes--) | Mendapatkan jumlah fast bytes yang digunakan untuk kompresi. |
### AppleLzmaCompressionSettings(int blockSize) {#AppleLzmaCompressionSettings-int-}
```
public AppleLzmaCompressionSettings(int blockSize)
```


Menginisialisasi sebuah instance baru dari kelas [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| blockSize | int | Ukuran setiap blok data sebelum kompresi. |

### AppleLzmaCompressionSettings(int blockSize, int dictionarySize) {#AppleLzmaCompressionSettings-int-int-}
```
public AppleLzmaCompressionSettings(int blockSize, int dictionarySize)
```


Menginisialisasi sebuah instance baru dari kelas [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| blockSize | int | Ukuran setiap blok data sebelum kompresi. |
| dictionarySize | int | Ukuran kamus yang digunakan untuk kompresi. |

### AppleLzmaCompressionSettings(int blockSize, int dictionarySize, int fastBytes) {#AppleLzmaCompressionSettings-int-int-int-}
```
public AppleLzmaCompressionSettings(int blockSize, int dictionarySize, int fastBytes)
```


Menginisialisasi sebuah instance baru dari kelas [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| blockSize | int | Ukuran setiap blok data sebelum kompresi. |
| dictionarySize | int | Ukuran kamus yang digunakan untuk kompresi. |
| fastBytes | int | Jumlah fast bytes yang digunakan untuk kompresi. |

### AppleLzmaCompressionSettings() {#AppleLzmaCompressionSettings--}
```
public AppleLzmaCompressionSettings()
```


Menginisialisasi sebuah instance baru dari kelas [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) dengan parameter default.

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


Mendapatkan ukuran setiap blok data sebelum kompresi.

Nilai: Nilai default adalah 4 MiB.

**Returns:**
int - ukuran setiap blok data sebelum kompresi.
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


Mendapatkan ukuran kamus yang digunakan untuk kompresi.

Nilai: Nilai default adalah 8 MiB.

**Returns:**
int - ukuran kamus yang digunakan untuk kompresi.
### getFastBytes() {#getFastBytes--}
```
public final int getFastBytes()
```


Mendapatkan jumlah fast bytes yang digunakan untuk kompresi.

Nilai: Nilai default adalah 32.

**Returns:**
int - jumlah fast bytes yang digunakan untuk kompresi.
