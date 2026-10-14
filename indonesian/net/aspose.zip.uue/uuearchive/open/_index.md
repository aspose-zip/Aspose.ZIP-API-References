---
title: "UueArchive.Open"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "UueArchive metode. Membuka arsip untuk dekripsi dan menyediakan stream dengan konten arsip"
type: docs
weight: 60
url: /id/net/aspose.zip.uue/uuearchive/open/
---
## UueArchive.Open method

Membuka arsip untuk decoding dan menyediakan aliran dengan konten arsip.

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

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


