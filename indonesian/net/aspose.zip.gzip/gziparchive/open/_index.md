---
title: GzipArchive.Open
second_title: Aspose.ZIP untuk Referensi .NET API
description: GzipArchive metode. Membuka arsip untuk ekstraksi dan menyediakan aliran dengan konten arsip.
type: docs
weight: 50
url: /id/net/aspose.zip.gzip/gziparchive/open/
---
## GzipArchive.Open method

Membuka arsip untuk ekstraksi dan menyediakan aliran dengan konten arsip.

```csharp
public Stream Open()
```

### Nilai Pengembalian

Aliran yang mewakili konten arsip.

### Perkataan

Baca dari aliran untuk mendapatkan konten asli file. Lihat bagian contoh.

### Contoh

Ekstrak arsip dan salin konten yang diekstraksi ke aliran file.

Anda dapat menggunakan metode Stream.CopyTo untuk .NET 4.0 dan lebih tinggi:

```csharp
unpacked.CopyTo(extracted);
```

```csharp
using (var archive = new GzipArchive("archive.gz"))
{
    using (var extracted = File.Create("data.bin"))
    {
        var unpacked = archive.Open();
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = unpacked.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }            
}
```

### Lihat juga

* class [GzipArchive](../)
* ruang nama [Aspose.Zip.Gzip](../../gziparchive/)
* perakitan [Aspose.Zip](../../../)


