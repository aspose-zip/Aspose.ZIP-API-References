---
title: "ParallelOptions.AvailableMemorySize"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Properti ParallelOptions. Mendapatkan atau mengatur perkiraan memori dalam megabyte yang tersedia untuk menampung entri terkompresi tanpa pertukaran ke disk. Nilai ini hanya masuk akal jika pengaturan ParallelCompressInMemory berada dalam mode Otomatis"
type: docs
weight: 20
url: /id/net/aspose.zip.saving/paralleloptions/availablememorysize/
---
## ParallelOptions.AvailableMemorySize property

Mendapatkan atau mengatur perkiraan memori dalam megabyte yang tersedia untuk menampung entri terkompresi tanpa pertukaran ke disk. Nilai ini hanya masuk akal jika pengaturan [`ParallelCompressInMemory`](../parallelcompressinmemory/) berada dalam mode Otomatis.

```csharp
public int AvailableMemorySize { get; set; }
```

## Catatan

Nilai ini digunakan untuk menghitung ukuran maksimum entri yang dapat dikompresi secara paralel dengan yang lain. Semua entri di atas ambang batas yang dihitung akan dikompresi secara berurutan. Aman untuk memiliki properti `AvailableMemorySize` sebesar RAM bebas bahkan lebih besar. Secara default, diasumsikan Anda memiliki setidaknya 200 MB per inti CPU.

### Lihat Juga

* class [ParallelOptions](../)
* namespace [Aspose.Zip.Saving](../../paralleloptions/)
* assembly [Aspose.Zip](../../../)


