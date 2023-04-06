---
title: Class ArchiveEntryPlain
second_title: Aspose.ZIP untuk Referensi .NET API
description: Aspose.Zip.ArchiveEntryPlain kelas. Entri zip yang perlu dikompresi tanpa enkripsi atau didekompresi tanpa dekripsi.
type: docs
weight: 40
url: /id/net/aspose.zip/archiveentryplain/
---
## ArchiveEntryPlain class

Entri zip yang perlu dikompresi tanpa enkripsi atau didekompresi tanpa dekripsi.

```csharp
public sealed class ArchiveEntryPlain : ArchiveEntry
```

## Properti

| Nama | Keterangan |
| --- | --- |
| [Comment](../../aspose.zip/archiveentry/comment/) { get; } | Mendapat komentar dari entri dalam arsip. |
| [CompressedSize](../../aspose.zip/archiveentry/compressedsize/) { get; } | Mendapat ukuran file terkompresi. |
| [CompressionSettings](../../aspose.zip/archiveentry/compressionsettings/) { get; } | Mendapat pengaturan untuk kompresi atau dekompresi. |
| [IsDirectory](../../aspose.zip/archiveentry/isdirectory/) { get; } | Mendapat nilai yang menunjukkan apakah entri mewakili direktori. |
| [ModificationTime](../../aspose.zip/archiveentry/modificationtime/) { get; set; } | Mendapat atau menyetel tanggal dan waktu terakhir diubah. |
| [Name](../../aspose.zip/archiveentry/name/) { get; } | Mendapat nama entri dalam arsip. |
| [UncompressedSize](../../aspose.zip/archiveentry/uncompressedsize/) { get; } | Mendapat ukuran file asli. |

## Metode

| Nama | Keterangan |
| --- | --- |
| [Extract](../../aspose.zip/archiveentry/extract/)(Stream, string) | Mengekstrak entri ke aliran yang disediakan. |
| [Extract](../../aspose.zip/archiveentry/extract/)(string, string) | Mengekstrak entri ke sistem file dengan jalur yang disediakan. |
| [Open](../../aspose.zip/archiveentry/open/)(string) | Membuka entri untuk ekstraksi dan menyediakan streaming dengan konten entri yang didekompresi. |

## Acara

| Nama | Keterangan |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip/archiveentry/compressionprogressed/) | Muncul saat sebagian aliran mentah dikompresi. |
| event [ExtractionProgressed](../../aspose.zip/archiveentry/extractionprogressed/) | Muncul saat sebagian aliran mentah diekstrak. |

### Lihat juga

* class [ArchiveEntry](../archiveentry/)
* ruang nama [Aspose.Zip](../../aspose.zip/)
* perakitan [Aspose.Zip](../../)


