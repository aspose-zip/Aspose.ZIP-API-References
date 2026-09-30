---
title: "ArchiveEntry.Open"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode ArchiveEntry. Membuka entri untuk ekstraksi dan menyediakan *stream* dengan konten entri yang terdekompresi."
type: docs
weight: 120
url: /id/net/aspose.zip/archiveentry/open/
---
## ArchiveEntry.Open method

Membuka entri untuk ekstraksi dan menyediakan aliran dengan konten entri yang didekompresi.

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
| InvalidOperationException | Arsip berada dalam keadaan yang tidak benar. |
| ObjectDisposedException | Dilempar jika arsip telah dibuang. |

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

* class [ArchiveEntry](../)
* namespace [Aspose.Zip](../../archiveentry/)
* assembly [Aspose.Zip](../../../)


