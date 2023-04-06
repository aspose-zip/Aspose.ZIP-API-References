---
title: Class ArchiveEntry
second_title: Aspose.ZIP untuk Referensi .NET API
description: Aspose.Zip.ArchiveEntry kelas. Merupakan file tunggal dalam arsip.
type: docs
weight: 20
url: /id/net/aspose.zip/archiveentry/
---
## ArchiveEntry class

Merupakan file tunggal dalam arsip.

```csharp
public abstract class ArchiveEntry : IArchiveFileEntry
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
| [Extract](../../aspose.zip/archiveentry/extract/#extract_1)(Stream, string) | Mengekstrak entri ke aliran yang disediakan. |
| [Extract](../../aspose.zip/archiveentry/extract/#extract)(string, string) | Mengekstrak entri ke sistem file dengan jalur yang disediakan. |
| [Open](../../aspose.zip/archiveentry/open/)(string) | Membuka entri untuk ekstraksi dan menyediakan streaming dengan konten entri yang didekompresi. |

## Acara

| Nama | Keterangan |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip/archiveentry/compressionprogressed/) | Muncul saat sebagian aliran mentah dikompresi. |
| event [ExtractionProgressed](../../aspose.zip/archiveentry/extractionprogressed/) | Muncul saat sebagian aliran mentah diekstrak. |

### Perkataan

Cast sebuah`ArchiveEntry` contoh ke[`ArchiveEntryEncrypted`](../archiveentryencrypted/) untuk menentukan apakah entri dienkripsi atau tidak.

### Lihat juga

* interface [IArchiveFileEntry](../iarchivefileentry/)
* ruang nama [Aspose.Zip](../../aspose.zip/)
* perakitan [Aspose.Zip](../../)


