---
title: Bzip2Archive.Open
second_title: Aspose.ZIP untuk Referensi .NET API
description: Bzip2Archive metode. Membuka arsip untuk ekstraksi dan menyediakan aliran dengan konten arsip.
type: docs
weight: 40
url: /id/net/aspose.zip.bzip2/bzip2archive/open/
---
## Bzip2Archive.Open method

Membuka arsip untuk ekstraksi dan menyediakan aliran dengan konten arsip.

```csharp
public Stream Open()
```

### Nilai Pengembalian

Aliran yang mewakili konten arsip.

### Perkataan

Baca dari aliran untuk mendapatkan konten asli file. Lihat bagian contoh.

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
Stream decompressed = archive.Open();
```

### Lihat juga

* class [Bzip2Archive](../)
* ruang nama [Aspose.Zip.Bzip2](../../bzip2archive/)
* perakitan [Aspose.Zip](../../../)


