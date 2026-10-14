---
title: "RarArchiveEntry.Open"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "RarArchiveEntry metode. Membuka entri untuk ekstraksi dan menyediakan aliran dengan konten entri yang didekompresi"
type: docs
weight: 100
url: /id/net/aspose.zip.rar/rararchiveentry/open/
---
## RarArchiveEntry.Open method

Membuka entri untuk ekstraksi dan menyediakan aliran dengan konten entri yang didekompresi.

```csharp
public Stream Open(string password = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| password | String | Kata sandi opsional untuk dekripsi. Itu juga dapat diatur dalam [`DecryptionPassword`](../../rararchiveloadoptions/decryptionpassword/). |

### Nilai Kembalian

Stream yang mewakili isi entri.

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

* class [RarArchiveEntry](../)
* namespace [Aspose.Zip.Rar](../../rararchiveentry/)
* assembly [Aspose.Zip](../../../)


