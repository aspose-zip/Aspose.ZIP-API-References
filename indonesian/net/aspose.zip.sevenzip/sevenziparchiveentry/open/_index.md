---
title: "SevenZipArchiveEntry.Open"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode SevenZipArchiveEntry. Membuka entri untuk ekstraksi dan menyediakan aliran dengan konten entri"
type: docs
weight: 90
url: /id/net/aspose.zip.sevenzip/sevenziparchiveentry/open/
---
## SevenZipArchiveEntry.Open method

Membuka entri untuk ekstraksi dan menyediakan aliran dengan konten entri.

```csharp
public Stream Open(string password = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| password | String | Password opsional untuk dekripsi. |

### Nilai Kembalian

Stream yang mewakili isi entri.

### Pengecualian

| exception | kondisi |
| --- | --- |
| InvalidOperationException | Arsip tidak dibuka untuk ekstraksi. - atau - Entri ini adalah direktori. |
| InvalidDataException | Data salah dalam entri. |
| ObjectDisposedException | Dilemparkan jika aliran sumber telah dibuang. |

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

* class [SevenZipArchiveEntry](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* assembly [Aspose.Zip](../../../)


