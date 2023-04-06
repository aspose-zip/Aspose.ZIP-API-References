---
title: SplitSevenZipArchiveSaveOptions.SplitSevenZipArchiveSaveOptions
second_title: Aspose.ZIP untuk Referensi .NET API
description: SplitSevenZipArchiveSaveOptions konstruktor. Instansi pengaturan untuk menyimpan arsip 7z multivolume.
type: docs
weight: 10
url: /id/net/aspose.zip.saving/splitsevenziparchivesaveoptions/splitsevenziparchivesaveoptions/
---
## SplitSevenZipArchiveSaveOptions constructor

Instansi pengaturan untuk menyimpan arsip 7z multi-volume.

```csharp
public SplitSevenZipArchiveSaveOptions(string fileName, uint segmentSize)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| fileName | String | Nama untuk volume. Mungkin dengan atau tanpa ekstensi .7z. |
| segmentSize | UInt32 | Ukuran volume. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentOutOfRangeException | *segmentSize* kurang dari 100. |

### Perkataan

Beberapa volume mungkin kurang dari*segmentSize*. Dalam kebanyakan kasus, segmen terakhir akan lebih sedikit tetapi segmen reguler juga jarang.

Nama file akan menjadi sebagai berikut:*fileName* .7z.001,*fileName* .7z.002, ...,*fileName*.7z.(n).

### Lihat juga

* class [SplitSevenZipArchiveSaveOptions](../)
* ruang nama [Aspose.Zip.Saving](../../splitsevenziparchivesaveoptions/)
* perakitan [Aspose.Zip](../../../)


