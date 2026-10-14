---
title: "Kelas ArchiveEntryEncrypted"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Kelas Aspose.Zip.ArchiveEntryEncrypted. Entri Zip yang perlu dikompres dengan enkripsi atau didekompres dengan dekripsi."
type: docs
weight: 180
url: /id/net/aspose.zip/archiveentryencrypted/
---
## ArchiveEntryEncrypted class

Entri zip yang perlu dikompresi dengan enkripsi atau didekompresi dengan dekripsi.

```csharp
public sealed class ArchiveEntryEncrypted : ArchiveEntry
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Comment](../../aspose.zip/archiveentry/comment/) { get; } | Mendapatkan komentar dari entri dalam arsip. |
| [CompressedSize](../../aspose.zip/archiveentry/compressedsize/) { get; } | Mendapatkan ukuran file terkompresi. |
| [CompressionSettings](../../aspose.zip/archiveentry/compressionsettings/) { get; } | Mendapatkan pengaturan untuk kompresi atau dekompresi. |
| [DataSource](../../aspose.zip/archiveentry/datasource/) { get; } | Sumber untuk entri jika entri tersebut ditambahkan ke arsip, bukan diekstrak. |
| [EncryptionSettings](../../aspose.zip/archiveentryencrypted/encryptionsettings/) { get; } | Mendapatkan pengaturan untuk enkripsi atau dekripsi. |
| [IsDirectory](../../aspose.zip/archiveentry/isdirectory/) { get; } | Mendapatkan nilai yang menunjukkan apakah entri mewakili sebuah direktori. |
| [ModificationTime](../../aspose.zip/archiveentry/modificationtime/) { get; set; } | Mendapatkan atau mengatur tanggal dan waktu terakhir diubah. |
| [Name](../../aspose.zip/archiveentry/name/) { get; } | Mendapatkan nama entri dalam arsip. |
| [UncompressedSize](../../aspose.zip/archiveentry/uncompressedsize/) { get; } | Mendapatkan ukuran file asli. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Extract](../../aspose.zip/archiveentry/extract/)(Stream, string) | Mengekstrak entri ke aliran yang disediakan. |
| [Extract](../../aspose.zip/archiveentry/extract/)(string, string) | Mengekstrak entri ke sistem file menggunakan jalur yang disediakan. |
| [Open](../../aspose.zip/archiveentry/open/)(string) | Membuka entri untuk ekstraksi dan menyediakan aliran dengan konten entri yang didekompresi. |

## Peristiwa

| Nama | Deskripsi |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip/archiveentry/compressionprogressed/) | Dipicu ketika sebagian aliran mentah dikompresi. |
| event [ExtractionProgressed](../../aspose.zip/archiveentry/extractionprogressed/) | Dipicu ketika sebagian aliran mentah diekstrak. |

### Lihat Juga

* class [ArchiveEntry](../archiveentry/)
* namespace [Aspose.Zip](../../aspose.zip/)
* assembly [Aspose.Zip](../../)


