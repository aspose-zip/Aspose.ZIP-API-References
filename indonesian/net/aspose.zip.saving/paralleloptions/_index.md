---
title: "Kelas ParallelOptions"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Kelas Aspose.Zip.Saving.ParallelOptions. Opsi untuk kompresi paralel"
type: docs
weight: 990
url: /id/net/aspose.zip.saving/paralleloptions/
---
## ParallelOptions class

Opsi untuk kompresi paralel.

```csharp
public class ParallelOptions
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [ParallelOptions](paralleloptions/)() | Konstruktor default. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [AvailableMemorySize](../../aspose.zip.saving/paralleloptions/availablememorysize/) { get; set; } | Mendapatkan atau mengatur perkiraan memori dalam megabyte yang tersedia untuk menampung entri terkompresi tanpa pertukaran ke disk. Nilai ini hanya masuk akal jika pengaturan [`ParallelCompressInMemory`](./parallelcompressinmemory/) berada dalam mode Otomatis. |
| [ParallelCompressInMemory](../../aspose.zip.saving/paralleloptions/parallelcompressinmemory/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan bagaimana pendekatan paralel akan digunakan. |

## Catatan

Opsi-opsi ini mengelola kompresi simultan oleh beberapa inti CPU.

## Contoh

```csharp
using (var archive = new Archive())
{
    archive.CreateEntries("DirToCompress");
    archive.Save("archive.zip", new ArchiveSaveOptions() { ParallelOptions = new ParallelOptions { ParallelCompressInMemory = ParallelCompressionMode.Auto, AvailableMemorySize = 4000 } });
}
```

### Lihat Juga

* namespace [Aspose.Zip.Saving](../../aspose.zip.saving/)
* assembly [Aspose.Zip](../../)


