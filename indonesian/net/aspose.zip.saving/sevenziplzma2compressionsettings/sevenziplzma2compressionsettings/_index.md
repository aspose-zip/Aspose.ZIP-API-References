---
title: "SevenZipLZMA2CompressionSettings.SevenZipLZMA2CompressionSettings"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Konstruktor SevenZipLZMA2CompressionSettings. Membuat instance pengaturan untuk metode kompresi LZMA2 dalam arsip 7z."
type: docs
weight: 10
url: /id/net/aspose.zip.saving/sevenziplzma2compressionsettings/sevenziplzma2compressionsettings/
---
## SevenZipLZMA2CompressionSettings(int) {#constructor}

Membuat instance pengaturan untuk metode kompresi LZMA2 dalam arsip 7z.

```csharp
public SevenZipLZMA2CompressionSettings(int dictionarySize = 16777216)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| dictionarySize | Int32 | Ukuran buffer riwayat harus berada di antara 4096 dan 1073741824. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentOutOfRangeException | *dictionarySize* terlalu besar atau terlalu kecil. |

## Catatan

Semakin besar kamus, biasanya rasio kompresi semakin baik - tetapi kamus yang lebih besar daripada data tidak terkompresi merupakan pemborosan RAM.

### Lihat Juga

* class [SevenZipLZMA2CompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../sevenziplzma2compressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## SevenZipLZMA2CompressionSettings(int, int) {#constructor_1}

Membuat instance pengaturan untuk metode kompresi LZMA2 dalam arsip 7z.

```csharp
public SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes = 32)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| dictionarySize | Int32 | Ukuran buffer riwayat harus berada di antara 4096 dan 1073741824. |
| fastBytes | Int32 | Mengontrol jumlah byte cepat yang digunakan oleh kompresor LZMA2. Jumlah byte cepat yang lebih besar dapat memberikan rasio kompresi yang lebih baik dengan mengorbankan kecepatan kompresi. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentOutOfRangeException | *dictionarySize* terlalu besar atau terlalu kecil, atau *fastBytes* terlalu besar atau terlalu kecil. |

## Catatan

Semakin besar kamus, biasanya rasio kompresi semakin baik - tetapi kamus yang lebih besar daripada data tidak terkompresi merupakan pemborosan RAM.

### Lihat Juga

* class [SevenZipLZMA2CompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../sevenziplzma2compressionsettings/)
* assembly [Aspose.Zip](../../../)


