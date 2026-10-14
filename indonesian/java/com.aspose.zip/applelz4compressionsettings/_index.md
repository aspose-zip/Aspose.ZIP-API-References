---
title: "AppleLz4CompressionSettings"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Pengaturan untuk kompresi LZ4 dalam file Apple Archive .aar."
type: docs
weight: 21
url: /id/java/com.aspose.zip/applelz4compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings)
```
public class AppleLz4CompressionSettings extends AppleCompressionSettings
```

Pengaturan untuk kompresi LZ4 dalam file Apple Archive (.aar).
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [AppleLz4CompressionSettings(int blockSize)](#AppleLz4CompressionSettings-int-) | Menginisialisasi sebuah instance baru dari kelas [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings). |
| [AppleLz4CompressionSettings()](#AppleLz4CompressionSettings--) | Menginisialisasi sebuah instance baru dari kelas [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings) dengan parameter default. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Mendapatkan ukuran setiap blok terkompresi `pbz4`/`bv41`. |
### AppleLz4CompressionSettings(int blockSize) {#AppleLz4CompressionSettings-int-}
```
public AppleLz4CompressionSettings(int blockSize)
```


Menginisialisasi sebuah instance baru dari kelas [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| blockSize | int | Ukuran setiap blok terkompresi `pbz4`/`bv41`. |

### AppleLz4CompressionSettings() {#AppleLz4CompressionSettings--}
```
public AppleLz4CompressionSettings()
```


Menginisialisasi sebuah instance baru dari kelas [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings) dengan parameter default.

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


Mendapatkan ukuran setiap blok terkompresi `pbz4`/`bv41`.

Nilai: Nilai default adalah 4 MiB.

**Returns:**
int - ukuran setiap blok terkompresi `pbz4`/`bv41`.
