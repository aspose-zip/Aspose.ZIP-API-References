---
title: "SevenZipPPMdCompressionSettings.SevenZipPPMdCompressionSettings"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Konstruktor SevenZipPPMdCompressionSettings. Membuat instansi pengaturan untuk metode kompresi PPMd dalam arsip 7z"
type: docs
weight: 10
url: /id/net/aspose.zip.saving/sevenzipppmdcompressionsettings/sevenzipppmdcompressionsettings/
---
## SevenZipPPMdCompressionSettings(byte, int) {#constructor_1}

Membuat instance pengaturan untuk metode kompresi PPMd dalam arsip 7z.

```csharp
public SevenZipPPMdCompressionSettings(byte maxOrder, int suballocatorSize)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| maxOrder | Byte | Urutan maksimum. |
| suballocatorSize | Int32 | Ukuran memori dalam MB yang dapat dikonsumsi oleh suballocator. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentOutOfRangeException | *maxOrder* tidak berada di antara 2 dan 32, atau *suballocatorSize* tidak berada di antara 1 dan 1024. |

## Catatan

Urutan model yang lebih besar hampir pasti menghasilkan kompresi yang lebih baik dan pasti menggunakan lebih banyak memori serta CPU.

Algoritma PPMd mungkin memerlukan banyak memori, terutama ketika digunakan pada file besar dan/atau dengan urutan model yang besar. Jika ppmd membutuhkan memori lebih banyak daripada yang Anda berikan, kompresi akan menjadi lebih buruk.

## Contoh

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings(4, 32))))
{
    archive.CreateEntry("data.bin", "data.bin");                        
    archive.Save(sevenZipFile);
 }
```

### Lihat Juga

* class [SevenZipPPMdCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../sevenzipppmdcompressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## SevenZipPPMdCompressionSettings() {#constructor}

Membuat instance pengaturan untuk metode kompresi PPMd dalam arsip 7z dengan urutan model default dan ukuran sub-allocator.

```csharp
public SevenZipPPMdCompressionSettings()
```

## Catatan

Urutan model default adalah 6 dan ukuran sub-allocator adalah 16MB.

## Contoh

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                        
    archive.Save(sevenZipFile);
 }
```

### Lihat Juga

* class [SevenZipPPMdCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../sevenzipppmdcompressionsettings/)
* assembly [Aspose.Zip](../../../)


