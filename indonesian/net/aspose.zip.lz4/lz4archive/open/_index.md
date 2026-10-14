---
title: "Lz4Archive.Open"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode Lz4Archive. Membuka arsip untuk ekstraksi dan menyediakan aliran dengan konten arsip."
type: docs
weight: 50
url: /id/net/aspose.zip.lz4/lz4archive/open/
---
## Lz4Archive.Open method

Membuka arsip untuk ekstraksi dan menyediakan aliran dengan konten arsip.

```csharp
public Stream Open()
```

### Nilai Kembalian

Stream yang mewakili isi arsip.

### Pengecualian

| exception | kondisi |
| --- | --- |
| EndOfStreamException | Aliran sumber terlalu pendek. |
| InvalidDataException | Byte yang salah ditemukan saat menginisialisasi dekoding. |
| InvalidOperationException | Arsip telah dipersiapkan untuk komposisi. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |
| IOException | Terjadi kesalahan I/O. |

## Catatan

Baca dari *stream* untuk mendapatkan konten asli sebuah file. Lihat bagian contoh.

## Contoh

Mengekstrak arsip dan menyalin konten yang diekstrak ke aliran file.

```csharp
using (var archive = new Lz4Archive("archive.lz4"))
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

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


