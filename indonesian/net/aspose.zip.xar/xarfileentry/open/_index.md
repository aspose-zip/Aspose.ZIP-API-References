---
title: XarFileEntry.Open
second_title: Aspose.ZIP untuk Referensi .NET API
description: XarFileEntry metode. Membuka entri untuk ekstraksi dan menyediakan aliran dengan konten entri.
type: docs
weight: 30
url: /id/net/aspose.zip.xar/xarfileentry/open/
---
## XarFileEntry.Open method

Membuka entri untuk ekstraksi dan menyediakan aliran dengan konten entri.

```csharp
public abstract Stream Open()
```

### Nilai Pengembalian

Aliran yang mewakili konten entri.

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
Stream decompressed = entry.Open();
```

### Lihat juga

* class [XarFileEntry](../)
* ruang nama [Aspose.Zip.Xar](../../xarfileentry/)
* perakitan [Aspose.Zip](../../../)


