---
title: "SplitSevenZipArchiveSaveOptions.SplitSevenZipArchiveSaveOptions"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Konstruktor SplitSevenZipArchiveSaveOptions. Membuat instance pengaturan untuk menyimpan arsip 7z multi-volume"
type: docs
weight: 10
url: /id/net/aspose.zip.saving/splitsevenziparchivesaveoptions/splitsevenziparchivesaveoptions/
---
## SplitSevenZipArchiveSaveOptions constructor

Membuat instance pengaturan untuk menyimpan arsip 7z multi-volume.

```csharp
public SplitSevenZipArchiveSaveOptions(string fileName, uint segmentSize)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fileName | String | Nama untuk volume. Bisa dengan atau tanpa ekstensi .7z. |
| segmentSize | UInt32 | Ukuran volume. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentOutOfRangeException | *segmentSize* kurang dari 100. |

## Catatan

Beberapa volume mungkin lebih kecil dari *segmentSize*. Dalam kebanyakan kasus, segmen terakhir akan lebih kecil tetapi jarang segmen reguler mungkin terlalu kecil.

Nama file akan menjadi sebagai berikut: *fileName*.7z.001, *fileName*.7z.002, ..., *fileName*.7z.(n).

### Lihat Juga

* class [SplitSevenZipArchiveSaveOptions](../)
* namespace [Aspose.Zip.Saving](../../splitsevenziparchivesaveoptions/)
* assembly [Aspose.Zip](../../../)


