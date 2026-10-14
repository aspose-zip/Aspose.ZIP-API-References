---
title: "GzipArchive.Open"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode GzipArchive. Membuka arsip untuk ekstraksi dan menyediakan aliran dengan konten arsip"
type: docs
weight: 70
url: /id/net/aspose.zip.gzip/gziparchive/open/
---
## GzipArchive.Open method

Membuka arsip untuk ekstraksi dan menyediakan aliran dengan konten arsip.

```csharp
public Stream Open()
```

### Nilai Kembalian

Stream yang mewakili isi arsip.

### Pengecualian

| exception | kondisi |
| --- | --- |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |

## Catatan

Baca dari *stream* untuk mendapatkan konten asli sebuah file. Lihat bagian contoh.

## Contoh

Mengekstrak arsip dan menyalin konten yang diekstrak ke aliran file.

```csharp
using (var archive = new GzipArchive("archive.gz"))
{
    using (var extracted = File.Create("data.bin"))
    {
        using(var unpacked = archive.Open())
        {
            byte[] b = new byte[8192];
            int bytesRead;
            while (0 < (bytesRead = unpacked.Read(b, 0, b.Length)))
                extracted.Write(b, 0, bytesRead);
        }
    }            
}
```

Anda dapat menggunakan metode Stream.CopyTo untuk .NET 4.0 ke atas:

```csharp
unpacked.CopyTo(extracted);
```

### Lihat Juga

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)


