---
title: "ZstandardArchive.Open"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "ZstandardArchive metode. Membuka arsip untuk ekstraksi dan menyediakan aliran dengan konten arsip."
type: docs
weight: 50
url: /id/net/aspose.zip.zstandard/zstandardarchive/open/
---
## ZstandardArchive.Open method

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
using (var archive = new ZstandardArchive("archive.zst"))
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

Anda dapat menggunakan metode Stream.CopyTo untuk .NET 4.0 ke atas:

```csharp
unpacked.CopyTo(extracted);
```

### Lihat Juga

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)


