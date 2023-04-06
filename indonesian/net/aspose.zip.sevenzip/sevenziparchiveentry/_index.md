---
title: Class SevenZipArchiveEntry
second_title: Aspose.ZIP untuk Referensi .NET API
description: Aspose.Zip.SevenZip.SevenZipArchiveEntry kelas. Merupakan file tunggal dalam arsip 7z.
type: docs
weight: 670
url: /id/net/aspose.zip.sevenzip/sevenziparchiveentry/
---
## SevenZipArchiveEntry class

Merupakan file tunggal dalam arsip 7z.

```csharp
public abstract class SevenZipArchiveEntry : IArchiveFileEntry
```

## Properti

| Nama | Keterangan |
| --- | --- |
| [CompressedSize](../../aspose.zip.sevenzip/sevenziparchiveentry/compressedsize/) { get; } | Mendapat ukuran file terkompresi. |
| [CompressionSettings](../../aspose.zip.sevenzip/sevenziparchiveentry/compressionsettings/) { get; } | Mendapat pengaturan untuk kompresi atau dekompresi. |
| [IsDirectory](../../aspose.zip.sevenzip/sevenziparchiveentry/isdirectory/) { get; } | Mendapat nilai yang menunjukkan apakah entri mewakili direktori. |
| [ModificationTime](../../aspose.zip.sevenzip/sevenziparchiveentry/modificationtime/) { get; } | Mendapatkan tanggal dan waktu terakhir diubah. |
| [Name](../../aspose.zip.sevenzip/sevenziparchiveentry/name/) { get; } | Mendapat nama entri dalam arsip. |
| [UncompressedSize](../../aspose.zip.sevenzip/sevenziparchiveentry/uncompressedsize/) { get; } | Mendapat ukuran file asli. |

## Metode

| Nama | Keterangan |
| --- | --- |
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/#extract_1)(Stream, string) | Mengekstrak entri ke aliran yang disediakan. |
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/#extract)(string, string) | Mengekstrak entri ke sistem file dengan jalur yang disediakan. |
| [Open](../../aspose.zip.sevenzip/sevenziparchiveentry/open/)(string) | Membuka entri untuk ekstraksi dan menyediakan aliran dengan konten entri. |

## Acara

| Nama | Keterangan |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip.sevenzip/sevenziparchiveentry/compressionprogressed/) | Muncul saat sebagian aliran mentah dikompresi. |

### Perkataan

Cast sebuah`SevenZipArchiveEntry` contoh ke[`SevenZipArchiveEntryEncrypted`](../sevenziparchiveentryencrypted/) untuk menentukan apakah entri dienkripsi atau tidak.

### Lihat juga

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* ruang nama [Aspose.Zip.SevenZip](../../aspose.zip.sevenzip/)
* perakitan [Aspose.Zip](../../)


