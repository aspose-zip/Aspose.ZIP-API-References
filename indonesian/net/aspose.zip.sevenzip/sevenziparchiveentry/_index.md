---
title: "Kelas SevenZipArchiveEntry"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Kelas Aspose.Zip.SevenZip.SevenZipArchiveEntry. Mewakili satu file tunggal dalam arsip 7z"
type: docs
weight: 1200
url: /id/net/aspose.zip.sevenzip/sevenziparchiveentry/
---
## SevenZipArchiveEntry class

Mewakili satu file di dalam arsip 7z.

```csharp
public abstract class SevenZipArchiveEntry : IArchiveFileEntry
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [CompressedSize](../../aspose.zip.sevenzip/sevenziparchiveentry/compressedsize/) { get; } | Mendapatkan ukuran file terkompresi. |
| [CompressionSettings](../../aspose.zip.sevenzip/sevenziparchiveentry/compressionsettings/) { get; } | Mendapatkan pengaturan untuk kompresi atau dekompresi. |
| [IsDirectory](../../aspose.zip.sevenzip/sevenziparchiveentry/isdirectory/) { get; } | Mendapatkan nilai yang menunjukkan apakah entri mewakili sebuah direktori. |
| [ModificationTime](../../aspose.zip.sevenzip/sevenziparchiveentry/modificationtime/) { get; } | Mendapatkan tanggal dan waktu terakhir dimodifikasi. |
| [Name](../../aspose.zip.sevenzip/sevenziparchiveentry/name/) { get; } | Mendapatkan nama entri dalam arsip. |
| [UncompressedSize](../../aspose.zip.sevenzip/sevenziparchiveentry/uncompressedsize/) { get; } | Mendapatkan ukuran file asli. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/#extract_1)(Stream, string) | Mengekstrak entri ke aliran yang disediakan. |
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/#extract)(string, string) | Mengekstrak entri ke sistem file menggunakan jalur yang disediakan. |
| [Open](../../aspose.zip.sevenzip/sevenziparchiveentry/open/)(string) | Membuka entri untuk ekstraksi dan menyediakan aliran dengan konten entri. |

## Peristiwa

| Nama | Deskripsi |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip.sevenzip/sevenziparchiveentry/compressionprogressed/) | Dipicu ketika sebagian aliran mentah dikompresi. |

## Catatan

Ubah tipe sebuah instance `SevenZipArchiveEntry` menjadi [`SevenZipArchiveEntryEncrypted`](../sevenziparchiveentryencrypted/) untuk menentukan apakah entri terenkripsi atau tidak.

### Lihat Juga

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.SevenZip](../../aspose.zip.sevenzip/)
* assembly [Aspose.Zip](../../)


