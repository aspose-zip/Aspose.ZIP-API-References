---
title: Class ParallelOptions
second_title: Aspose.ZIP untuk Referensi .NET API
description: Aspose.Zip.Saving.ParallelOptions kelas. Opsi untuk kompresi paralel.
type: docs
weight: 490
url: /id/net/aspose.zip.saving/paralleloptions/
---
## ParallelOptions class

Opsi untuk kompresi paralel.

```csharp
public class ParallelOptions
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [ParallelOptions](paralleloptions/)() | Konstruktor default. |

## Properti

| Nama | Keterangan |
| --- | --- |
| [AvailableMemorySize](../../aspose.zip.saving/paralleloptions/availablememorysize/) { get; set; } | Mendapat atau menyetel perkiraan memori dalam megabyte yang tersedia untuk mengakomodasi entri terkompresi tanpa menukar ke disk. Nilai ini hanya masuk akal jika[`ParallelCompressInMemory`](./parallelcompressinmemory/) pengaturan sudah masukAuto mode. |
| [ParallelCompressInMemory](../../aspose.zip.saving/paralleloptions/parallelcompressinmemory/) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan bagaimana pendekatan paralel digunakan. |

### Perkataan

Opsi ini mengelola kompresi simultan oleh beberapa inti CPU.

### Contoh

```csharp
using (var archive = new Archive())
{
    archive.CreateEntries("DirToCompress");
    archive.Save("archive.zip", new ArchiveSaveOptions() { ParallelOptions = new ParallelOptions { ParallelCompressInMemory = mode, AvailableMemorySize = 4000 } });
}
```

### Lihat juga

* ruang nama [Aspose.Zip.Saving](../../aspose.zip.saving/)
* perakitan [Aspose.Zip](../../)


