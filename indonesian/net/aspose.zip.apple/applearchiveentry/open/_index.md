---
title: "AppleArchiveEntry.Open"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode AppleArchiveEntry. Membuka entri untuk ekstraksi dan menyediakan aliran dengan konten entri"
type: docs
weight: 60
url: /id/net/aspose.zip.apple/applearchiveentry/open/
---
## AppleArchiveEntry.Open method

Membuka entri untuk ekstraksi dan menyediakan aliran dengan konten entri.

```csharp
public Stream Open()
```

### Nilai Kembalian

Aliran yang dapat dibaca yang berisi data entri yang diekstrak.

### Pengecualian

| exception | kondisi |
| --- | --- |
| NotSupportedException | Entri ini termasuk dalam Apple Archive solid atau menggunakan metode kompresi yang tidak didukung. |
| InvalidDataException | Checksum atau digest yang disimpan untuk entri tidak cocok dengan data yang diekstrak. |
| InvalidOperationException | Entri ini termasuk dalam arsip yang disiapkan untuk komposisi, atau data entri tidak dapat dibuka dari aliran arsip yang tidak dapat dipindai. |
| ObjectDisposedException | Aliran sumber telah dibuang. |
| IOException | Terjadi kesalahan I/O. |

## Catatan

Baca dari aliran yang dikembalikan untuk memperoleh konten entri asli. Jika arsip berisi bidang checksum, checksum diverifikasi saat aliran yang dikembalikan dibaca.

### Lihat Juga

* class [AppleArchiveEntry](../)
* namespace [Aspose.Zip.Apple](../../applearchiveentry/)
* assembly [Aspose.Zip](../../../)


