---
title: PPMdCompressionSettings.PPMdCompressionSettings
second_title: Aspose.ZIP untuk Referensi .NET API
description: PPMdCompressionSettings konstruktor. Menginisialisasi instance baru dariPPMdCompressionSettings kelas.
type: docs
weight: 10
url: /id/net/aspose.zip.saving/ppmdcompressionsettings/ppmdcompressionsettings/
---
## PPMdCompressionSettings(int, int) {#constructor_1}

Menginisialisasi instance baru dari[`PPMdCompressionSettings`](../) kelas.

```csharp
public PPMdCompressionSettings(int modelOrder, int suballocatorSize)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| modelOrder | Int32 | Urutan model. |
| suballocatorSize | Int32 | Ukuran memori dalam MB suballocator dapat dikonsumsi. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentOutOfRangeException | *modelOrder* bukan antara 2 dan 16. - atau -*suballocatorSize* bukan antara 1 dan 256. |

### Perkataan

Pesanan model yang lebih besar hampir pasti menghasilkan kompresi yang lebih baik dan tentu saja lebih banyak penggunaan memori dan CPU.

Algoritme PPMd mungkin membutuhkan banyak memori, terutama bila digunakan pada file besar dan/atau digunakan dengan urutan model besar. Jika ppmd membutuhkan lebih banyak memori daripada yang Anda berikan, kompresi akan lebih buruk.

### Contoh

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings(4, 10))))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### Lihat juga

* class [PPMdCompressionSettings](../)
* ruang nama [Aspose.Zip.Saving](../../ppmdcompressionsettings/)
* perakitan [Aspose.Zip](../../../)

---

## PPMdCompressionSettings() {#constructor}

Menginisialisasi instance baru dari[`PPMdCompressionSettings`](../) kelas dengan urutan model default dan ukuran sub-allocator.

```csharp
public PPMdCompressionSettings()
```

### Perkataan

Urutan model default adalah 8 dan ukuran sub-alokator adalah 50MB.

### Contoh

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### Lihat juga

* class [PPMdCompressionSettings](../)
* ruang nama [Aspose.Zip.Saving](../../ppmdcompressionsettings/)
* perakitan [Aspose.Zip](../../../)


