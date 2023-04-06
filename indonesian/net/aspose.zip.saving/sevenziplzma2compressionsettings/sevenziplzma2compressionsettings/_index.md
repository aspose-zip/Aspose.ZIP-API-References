---
title: SevenZipLZMA2CompressionSettings.SevenZipLZMA2CompressionSettings
second_title: Aspose.ZIP untuk Referensi .NET API
description: SevenZipLZMA2CompressionSettings konstruktor. Membuat pengaturan untuk metode kompresi LZMA2 dalam arsip 7z.
type: docs
weight: 10
url: /id/net/aspose.zip.saving/sevenziplzma2compressionsettings/sevenziplzma2compressionsettings/
---
## SevenZipLZMA2CompressionSettings(int) {#constructor}

Membuat pengaturan untuk metode kompresi LZMA2 dalam arsip 7z.

```csharp
public SevenZipLZMA2CompressionSettings(int dictionarySize = 16777216)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| dictionarySize | Int32 | Ukuran buffer histori, harus antara 4096 dan 1073741824. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentOutOfRangeException | *dictionarySize* terlalu besar atau terlalu kecil. |

### Perkataan

Semakin besar kamusnya, biasanya semakin baik rasio kompresinya, tetapi kamus yang lebih besar dari data yang tidak terkompresi adalah pemborosan RAM.

### Lihat juga

* class [SevenZipLZMA2CompressionSettings](../)
* ruang nama [Aspose.Zip.Saving](../../sevenziplzma2compressionsettings/)
* perakitan [Aspose.Zip](../../../)

---

## SevenZipLZMA2CompressionSettings(int, int) {#constructor_1}

Membuat pengaturan untuk metode kompresi LZMA2 dalam arsip 7z.

```csharp
public SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes = 32)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| dictionarySize | Int32 | Ukuran buffer histori, harus antara 4096 dan 1073741824. |
| fastBytes | Int32 | Mengontrol jumlah byte cepat yang digunakan oleh kompresor LZMA2. Jumlah byte cepat yang lebih besar dapat memberikan rasio kompresi yang lebih baik dengan mengorbankan kecepatan kompresi. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentOutOfRangeException | *dictionarySize* terlalu besar atau terlalu kecil, atau*fastBytes* terlalu besar atau terlalu kecil. |

### Perkataan

Semakin besar kamusnya, biasanya semakin baik rasio kompresinya, tetapi kamus yang lebih besar dari data yang tidak terkompresi adalah pemborosan RAM.

### Lihat juga

* class [SevenZipLZMA2CompressionSettings](../)
* ruang nama [Aspose.Zip.Saving](../../sevenziplzma2compressionsettings/)
* perakitan [Aspose.Zip](../../../)


