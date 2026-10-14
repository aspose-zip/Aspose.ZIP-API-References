---
title: "Kelas XarFileEntry"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Kelas Aspose.Zip.Xar.XarFileEntry. Mewakili entri file dalam arsip xar"
type: docs
weight: 1470
url: /id/net/aspose.zip.xar/xarfileentry/
---
## XarFileEntry class

Mewakili entri file dalam arsip xar.

```csharp
public sealed class XarFileEntry : XarEntry, IArchiveFileEntry
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [CreationTime](../../aspose.zip.xar/xarentry/creationtime/) { get; } | Mendapatkan waktu pembuatan file atau direktori. |
| [FullPath](../../aspose.zip.xar/xarentry/fullpath/) { get; } | Mendapatkan jalur lengkap dari entri dalam arsip. |
| [IsDirectory](../../aspose.zip.xar/xarentry/isdirectory/) { get; } | Mendapatkan nilai yang menunjukkan apakah entri mewakili sebuah direktori. |
| [LastAccessTime](../../aspose.zip.xar/xarentry/lastaccesstime/) { get; } | Mendapatkan waktu akses terakhir file atau direktori. |
| [Length](../../aspose.zip.xar/xarfileentry/length/) { get; } | Mendapatkan panjang entri dalam byte. |
| [ModificationTime](../../aspose.zip.xar/xarentry/modificationtime/) { get; } | Mendapatkan waktu modifikasi file atau direktori. |
| [Name](../../aspose.zip.xar/xarentry/name/) { get; } | Mendapatkan nama entri dalam arsip. |
| [Parent](../../aspose.zip.xar/xarentry/parent/) { get; } | Mendapatkan direktori induk tempat entri berada. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Extract](../../aspose.zip.xar/xarfileentry/extract/#extract_1)(Stream) | Mengekstrak entri ke aliran yang disediakan. |
| [Extract](../../aspose.zip.xar/xarfileentry/extract/#extract)(string) | Mengekstrak entri ke sistem file menggunakan jalur yang disediakan. |
| [Open](../../aspose.zip.xar/xarfileentry/open/)() | Membuka entri untuk ekstraksi dan menyediakan aliran dengan konten entri. |
| override [ToString](../../aspose.zip.xar/xarentry/tostring/)() |  |

## Peristiwa

| Nama | Deskripsi |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip.xar/xarfileentry/compressionprogressed/) | Dipicu ketika sebagian aliran mentah dikompresi. |

### Lihat Juga

* class [XarEntry](../xarentry/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Xar](../../aspose.zip.xar/)
* assembly [Aspose.Zip](../../)


