---
title: SplitArchiveSaveOptions.SplitArchiveSaveOptions
second_title: Aspose.ZIP untuk Referensi .NET API
description: SplitArchiveSaveOptions konstruktor. Pengaturan instantiate untuk menyimpan arsip zip multivolume.
type: docs
weight: 10
url: /id/net/aspose.zip.saving/splitarchivesaveoptions/splitarchivesaveoptions/
---
## SplitArchiveSaveOptions constructor

Pengaturan instantiate untuk menyimpan arsip zip multi-volume.

```csharp
public SplitArchiveSaveOptions(string fileName, uint segmentSize)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| fileName | String | Nama untuk volume. Mungkin dengan atau tanpa ekstensi .zip. |
| segmentSize | UInt32 | Ukuran volume. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentOutOfRangeException | Ukuran segmen kurang dari 65536 byte. |

### Perkataan

Beberapa volume mungkin kurang dari*segmentSize*. Dalam kebanyakan kasus, segmen terakhir akan lebih sedikit tetapi segmen reguler juga jarang.

Nama file akan menjadi sebagai berikut:*fileName* .z01,*fileName* .z02, ...,*fileName* .z(n-1),*fileName*.ritsleting.

### Lihat juga

* class [SplitArchiveSaveOptions](../)
* ruang nama [Aspose.Zip.Saving](../../splitarchivesaveoptions/)
* perakitan [Aspose.Zip](../../../)


