---
title: "Bzip2Archive.Open"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode Bzip2Archive. Membuka arsip untuk ekstraksi dan menyediakan aliran dengan konten arsip."
type: docs
weight: 50
url: /id/net/aspose.zip.bzip2/bzip2archive/open/
---
## Bzip2Archive.Open method

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

Baca dari aliran untuk mendapatkan konten asli file. Lihat bagian contoh.

## Contoh

Penggunaan:

```csharp
Stream decompressed = archive.Open();
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

* class [Bzip2Archive](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2archive/)
* assembly [Aspose.Zip](../../../)


