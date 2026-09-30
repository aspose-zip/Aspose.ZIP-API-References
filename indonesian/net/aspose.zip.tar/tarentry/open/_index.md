---
title: "TarEntry.Open"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode TarEntry. Membuka entri untuk ekstraksi dan menyediakan aliran dengan konten entri"
type: docs
weight: 70
url: /id/net/aspose.zip.tar/tarentry/open/
---
## TarEntry.Open method

Membuka entri untuk ekstraksi dan menyediakan aliran dengan konten entri.

```csharp
public Stream Open()
```

### Nilai Kembalian

Stream yang mewakili isi entri.

### Pengecualian

| exception | kondisi |
| --- | --- |
| ObjectDisposedException | Dilemparkan jika aliran sumber telah dibuang. |
| IOException | Terjadi kesalahan I/O. |

## Catatan

Baca dari *stream* untuk mendapatkan konten asli sebuah file. Lihat bagian contoh.

## Contoh

Penggunaan:

```csharp
Stream decompressed = entry.Open();
```

.NET 4.0 ke atas - gunakan metode Stream.CopyTo:

```csharp
decompressed.CopyTo(httpResponse.OutputStream)
```

.NET 3.5 ke bawah - salin byte secara manual:

```csharp
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.Read(buffer, 0, buffer.Length)))
 fileStream.Write(buffer, 0, bytesRead);
```

### Lihat Juga

* class [TarEntry](../)
* namespace [Aspose.Zip.Tar](../../tarentry/)
* assembly [Aspose.Zip](../../../)


