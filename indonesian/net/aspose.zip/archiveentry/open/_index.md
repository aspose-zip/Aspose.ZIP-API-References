---
title: ArchiveEntry.Open
second_title: Aspose.ZIP untuk Referensi .NET API
description: ArchiveEntry metode. Membuka entri untuk ekstraksi dan menyediakan streaming dengan konten entri yang didekompresi.
type: docs
weight: 110
url: /id/net/aspose.zip/archiveentry/open/
---
## ArchiveEntry.Open method

Membuka entri untuk ekstraksi dan menyediakan streaming dengan konten entri yang didekompresi.

```csharp
public Stream Open(string password = null)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| password | String | Kata sandi opsional untuk dekripsi. |

### Nilai Pengembalian

Aliran yang mewakili konten entri.

### Perkataan

Baca dari aliran untuk mendapatkan konten asli dari file. Lihat bagian contoh.

### Contoh

Penggunaan:

.NET 4.0 dan lebih tinggi - gunakan metode Stream.CopyTo:

```csharp
decompressed.CopyTo(httpResponse.OutputStream)
```

.NET 3.5 dan sebelumnya - salin byte secara manual:

```csharp
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.Read(buffer, 0, buffer.Length)))
 fileStream.Write(buffer, 0, bytesRead);
```

```csharp
Stream decompressed = entry.Open();
```

### Lihat juga

* class [ArchiveEntry](../)
* ruang nama [Aspose.Zip](../../archiveentry/)
* perakitan [Aspose.Zip](../../../)


