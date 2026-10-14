---
title: "Kelas RarArchiveEntry"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Kelas Aspose.Zip.Rar.RarArchiveEntry. Mewakili satu file tunggal dalam arsip"
type: docs
weight: 800
url: /id/net/aspose.zip.rar/rararchiveentry/
---
## RarArchiveEntry class

Mewakili satu berkas dalam arsip.

```csharp
public abstract class RarArchiveEntry : IArchiveFileEntry
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [CompressedSize](../../aspose.zip.rar/rararchiveentry/compressedsize/) { get; } | Mendapatkan ukuran file terkompresi. |
| [CreationTime](../../aspose.zip.rar/rararchiveentry/creationtime/) { get; } | Mendapatkan tanggal dan waktu pembuatan. |
| [IsDirectory](../../aspose.zip.rar/rararchiveentry/isdirectory/) { get; } | Mendapatkan nilai yang menunjukkan apakah entri mewakili sebuah direktori. |
| [LastAccessTime](../../aspose.zip.rar/rararchiveentry/lastaccesstime/) { get; } | Mendapatkan tanggal dan waktu akses terakhir. |
| [ModificationTime](../../aspose.zip.rar/rararchiveentry/modificationtime/) { get; } | Mendapatkan tanggal dan waktu terakhir dimodifikasi. |
| [Name](../../aspose.zip.rar/rararchiveentry/name/) { get; } | Mendapatkan nama entri dalam arsip. |
| [UncompressedSize](../../aspose.zip.rar/rararchiveentry/uncompressedsize/) { get; } | Mendapatkan ukuran file asli. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Extract](../../aspose.zip.rar/rararchiveentry/extract/#extract_1)(Stream, string) | Mengekstrak entri ke aliran yang disediakan. |
| [Extract](../../aspose.zip.rar/rararchiveentry/extract/#extract)(string, string) | Mengekstrak entri ke sistem file menggunakan jalur yang disediakan. |
| [Open](../../aspose.zip.rar/rararchiveentry/open/)(string) | Membuka entri untuk ekstraksi dan menyediakan aliran dengan konten entri yang didekompresi. |

## Peristiwa

| Nama | Deskripsi |
| --- | --- |
| event [ExtractionProgressed](../../aspose.zip.rar/rararchiveentry/extractionprogressed/) | Dipicu ketika sebagian aliran mentah diekstrak. |

## Catatan

Ubah tipe instance `RarArchiveEntry` menjadi [`RarArchiveEntryEncrypted`](../rararchiveentryencrypted/) untuk menentukan apakah entri terenkripsi atau tidak.

### Lihat Juga

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Rar](../../aspose.zip.rar/)
* assembly [Aspose.Zip](../../)


