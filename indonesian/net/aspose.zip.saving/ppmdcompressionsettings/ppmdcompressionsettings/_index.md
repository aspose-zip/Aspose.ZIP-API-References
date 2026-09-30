---
title: "PPMdCompressionSettings.PPMdCompressionSettings"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Konstruktor PPMdCompressionSettings. Menginisialisasi instance baru dari kelas PPMdCompressionSettings"
type: docs
weight: 10
url: /id/net/aspose.zip.saving/ppmdcompressionsettings/ppmdcompressionsettings/
---
## PPMdCompressionSettings(int, int) {#constructor_1}

Menginisialisasi instance baru dari kelas [`PPMdCompressionSettings`](../).

```csharp
public PPMdCompressionSettings(int modelOrder, int suballocatorSize)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| modelOrder | Int32 | Urutan model. |
| suballocatorSize | Int32 | Ukuran memori dalam MB yang dapat dikonsumsi oleh suballocator. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentOutOfRangeException | *modelOrder* tidak berada di antara 2 dan 16. - atau - *suballocatorSize* tidak berada di antara 1 dan 256. |

## Catatan

Urutan model yang lebih besar hampir pasti menghasilkan kompresi yang lebih baik dan pasti menggunakan lebih banyak memori serta CPU.

Algoritma PPMd mungkin memerlukan banyak memori, terutama ketika digunakan pada file besar dan/atau dengan urutan model yang besar. Jika ppmd membutuhkan memori lebih banyak daripada yang Anda berikan, kompresi akan menjadi lebih buruk.

## Contoh

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings(4, 10))))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### Lihat Juga

* class [PPMdCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../ppmdcompressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## PPMdCompressionSettings() {#constructor}

Menginisialisasi instance baru dari kelas [`PPMdCompressionSettings`](../) dengan urutan model default dan ukuran sub-allocator.

```csharp
public PPMdCompressionSettings()
```

## Catatan

Urutan model default adalah 8, dan ukuran sub-allocator adalah 50MB.

## Contoh

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### Lihat Juga

* class [PPMdCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../ppmdcompressionsettings/)
* assembly [Aspose.Zip](../../../)


