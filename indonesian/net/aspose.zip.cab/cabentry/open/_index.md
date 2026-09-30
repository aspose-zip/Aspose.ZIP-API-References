---
title: "CabEntry.Open"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "CabEntry metode. Membuka entri untuk ekstraksi dan menyediakan aliran dengan konten entri"
type: docs
weight: 50
url: /id/net/aspose.zip.cab/cabentry/open/
---
## CabEntry.Open method

Membuka entri untuk ekstraksi dan menyediakan aliran dengan konten entri.

```csharp
public Stream Open()
```

### Nilai Kembalian

Stream yang mewakili isi entri.

### Pengecualian

| exception | kondisi |
| --- | --- |
| NotSupportedException | Inisialisasi aliran gagal karena data yang salah. |
| InvalidDataException | Arsip rusak. |
| InvalidOperationException | Entri tersebut termasuk dalam arsip yang disiapkan untuk komposisi. |
| ObjectDisposedException | Dilemparkan jika sumber telah dibuang. |
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

* class [CabEntry](../)
* namespace [Aspose.Zip.Cab](../../cabentry/)
* assembly [Aspose.Zip](../../../)


