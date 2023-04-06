---
title: ParallelOptions.AvailableMemorySize
second_title: Aspose.ZIP untuk Referensi .NET API
description: ParallelOptions Properti. Mendapat atau menyetel perkiraan memori dalam megabyte yang tersedia untuk mengakomodasi entri terkompresi tanpa menukar ke disk. Nilai ini hanya masuk akal jikaParallelCompressInMemory pengaturan sudah masukAuto mode.
type: docs
weight: 20
url: /id/net/aspose.zip.saving/paralleloptions/availablememorysize/
---
## ParallelOptions.AvailableMemorySize property

Mendapat atau menyetel perkiraan memori dalam megabyte yang tersedia untuk mengakomodasi entri terkompresi tanpa menukar ke disk. Nilai ini hanya masuk akal jika[`ParallelCompressInMemory`](../parallelcompressinmemory/) pengaturan sudah masukAuto mode.

```csharp
public int AvailableMemorySize { get; set; }
```

### Perkataan

Nilai ini digunakan untuk menghitung ukuran entri terbesar yang dapat dikompresi secara paralel dengan yang lain. Semua entri di atas ambang yang dihitung akan dikompresi secara berurutan. Aman untuk dimiliki`AvailableMemorySize` properti sebesar RAM gratis dan bahkan lebih besar. Secara default diasumsikan Anda memiliki setidaknya 200MB per inti CPU.

### Lihat juga

* class [ParallelOptions](../)
* ruang nama [Aspose.Zip.Saving](../../paralleloptions/)
* perakitan [Aspose.Zip](../../../)


