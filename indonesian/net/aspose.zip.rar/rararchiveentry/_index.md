---
title: Class RarArchiveEntry
second_title: Aspose.ZIP untuk Referensi .NET API
description: Aspose.Zip.Rar.RarArchiveEntry kelas. Merupakan file tunggal dalam arsip.
type: docs
weight: 320
url: /id/net/aspose.zip.rar/rararchiveentry/
---
## RarArchiveEntry class

Merupakan file tunggal dalam arsip.

```csharp
public abstract class RarArchiveEntry : IArchiveFileEntry
```

## Properti

| Nama | Keterangan |
| --- | --- |
| [CompressedSize](../../aspose.zip.rar/rararchiveentry/compressedsize/) { get; } | Mendapat ukuran file terkompresi. |
| [CreationTime](../../aspose.zip.rar/rararchiveentry/creationtime/) { get; } | Mendapat tanggal dan waktu pembuatan. |
| [IsDirectory](../../aspose.zip.rar/rararchiveentry/isdirectory/) { get; } | Mendapat nilai yang menunjukkan apakah entri mewakili direktori. |
| [LastAccessTime](../../aspose.zip.rar/rararchiveentry/lastaccesstime/) { get; } | Mendapat tanggal dan waktu akses terakhir. |
| [ModificationTime](../../aspose.zip.rar/rararchiveentry/modificationtime/) { get; } | Mendapatkan tanggal dan waktu terakhir diubah. |
| [Name](../../aspose.zip.rar/rararchiveentry/name/) { get; } | Mendapat nama entri dalam arsip. |
| [UncompressedSize](../../aspose.zip.rar/rararchiveentry/uncompressedsize/) { get; } | Mendapat ukuran file asli. |

## Metode

| Nama | Keterangan |
| --- | --- |
| [Extract](../../aspose.zip.rar/rararchiveentry/extract/#extract_1)(Stream, string) | Mengekstrak entri ke aliran yang disediakan. |
| [Extract](../../aspose.zip.rar/rararchiveentry/extract/#extract)(string, string) | Mengekstrak entri ke sistem file dengan jalur yang disediakan. |
| [Open](../../aspose.zip.rar/rararchiveentry/open/)(string) | Membuka entri untuk ekstraksi dan menyediakan streaming dengan konten entri yang didekompresi. |

## Acara

| Nama | Keterangan |
| --- | --- |
| event [ExtractionProgressed](../../aspose.zip.rar/rararchiveentry/extractionprogressed/) | Muncul saat sebagian aliran mentah diekstrak. |

### Perkataan

Cast a`RarArchiveEntry` contoh ke[`RarArchiveEntryEncrypted`](../rararchiveentryencrypted/) untuk menentukan apakah entri dienkripsi atau tidak.

### Lihat juga

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* ruang nama [Aspose.Zip.Rar](../../aspose.zip.rar/)
* perakitan [Aspose.Zip](../../)


