---
title: SevenZipPPMdCompressionSettings.SevenZipPPMdCompressionSettings
second_title: Aspose.ZIP untuk Referensi .NET API
description: SevenZipPPMdCompressionSettings konstruktor. Instansiasi pengaturan untuk metode kompresi PPMd dalam arsip 7z.
type: docs
weight: 10
url: /id/net/aspose.zip.saving/sevenzipppmdcompressionsettings/sevenzipppmdcompressionsettings/
---
## SevenZipPPMdCompressionSettings(byte, int) {#constructor_1}

Instansiasi pengaturan untuk metode kompresi PPMd dalam arsip 7z.

```csharp
public SevenZipPPMdCompressionSettings(byte maxOrder, int suballocatorSize)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| maxOrder | Byte | Pesanan maksimum. |
| suballocatorSize | Int32 | Ukuran memori dalam MB suballocator dapat dikonsumsi. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentOutOfRangeException | *maxOrder* tidak antara 2 dan 32, atau*suballocatorSize* bukan antara 1 dan 1024. |

### Perkataan

Pesanan model yang lebih besar hampir pasti menghasilkan kompresi yang lebih baik dan tentu saja lebih banyak penggunaan memori dan CPU.

Algoritme PPMd mungkin membutuhkan banyak memori, terutama bila digunakan pada file besar dan/atau digunakan dengan urutan model besar. Jika ppmd membutuhkan lebih banyak memori daripada yang Anda berikan, kompresi akan lebih buruk.

### Contoh

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings(4, 32))))
{
    archive.CreateEntry("data.bin", "data.bin");                        
    archive.Save(sevenZipFile);
 }
```

### Lihat juga

* class [SevenZipPPMdCompressionSettings](../)
* ruang nama [Aspose.Zip.Saving](../../sevenzipppmdcompressionsettings/)
* perakitan [Aspose.Zip](../../../)

---

## SevenZipPPMdCompressionSettings() {#constructor}

Instansi pengaturan untuk metode kompresi PPMd dalam arsip 7z dengan urutan model default dan ukuran sub-alokator.

```csharp
public SevenZipPPMdCompressionSettings()
```

### Perkataan

Urutan model default adalah 6 dan ukuran sub-alokator adalah 16 MB.

### Contoh

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                        
    archive.Save(sevenZipFile);
 }
```

### Lihat juga

* class [SevenZipPPMdCompressionSettings](../)
* ruang nama [Aspose.Zip.Saving](../../sevenzipppmdcompressionsettings/)
* perakitan [Aspose.Zip](../../../)


