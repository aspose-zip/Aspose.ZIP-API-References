---
title: "Kelas WimFileEntry"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Kelas Aspose.Zip.Wim.WimFileEntry. Mewakili satu file dalam arsip wim"
type: docs
weight: 1360
url: /id/net/aspose.zip.wim/wimfileentry/
---
## WimFileEntry class

Mewakili satu file dalam arsip wim.

```csharp
public sealed class WimFileEntry : WimEntry, IArchiveFileEntry
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [AlternateDataStreams](../../aspose.zip.wim/wimentry/alternatedatastreams/) { get; } | Mendapatkan nama-nama aliran data alternatif untuk sebuah file atau direktori. |
| [Archive](../../aspose.zip.wim/wimentry/archive/) { get; } | Mendapatkan arsip tempat entri tersebut berada. |
| [ChangeTime](../../aspose.zip.wim/wimentry/changetime/) { get; } | Mendapatkan waktu terakhir file atau direktori diubah. |
| [CreationTime](../../aspose.zip.wim/wimentry/creationtime/) { get; } | Mendapatkan waktu pembuatan file atau direktori. |
| [FileAttributes](../../aspose.zip.wim/wimentry/fileattributes/) { get; } | Mendapatkan atribut file atau direktori. |
| [FullPath](../../aspose.zip.wim/wimentry/fullpath/) { get; } | Mendapatkan jalur lengkap entri dalam citra. |
| [HardLink](../../aspose.zip.wim/wimentry/hardlink/) { get; } | Mendapatkan ID hardlink dari file atau direktori. |
| [HasHardLinks](../../aspose.zip.wim/wimentry/hashardlinks/) { get; } | Mendapatkan apakah file atau direktori dikenal dengan nama lain. |
| [Image](../../aspose.zip.wim/wimentry/image/) { get; } | Mendapatkan citra tempat entri tersebut berada. |
| [IsDirectory](../../aspose.zip.wim/wimentry/isdirectory/) { get; } | Mendapatkan nilai yang menunjukkan apakah entri mewakili sebuah direktori. |
| [LastAccessTime](../../aspose.zip.wim/wimentry/lastaccesstime/) { get; } | Mendapatkan waktu akses terakhir file atau direktori. |
| [Length](../../aspose.zip.wim/wimfileentry/length/) { get; } | Mendapatkan panjang entri dalam byte. |
| [ModificationTime](../../aspose.zip.wim/wimentry/modificationtime/) { get; } | Mendapatkan waktu modifikasi file atau direktori. |
| [Name](../../aspose.zip.wim/wimentry/name/) { get; } | Mendapatkan nama entri dalam citra. |
| [Parent](../../aspose.zip.wim/wimentry/parent/) { get; } | Mendapatkan direktori induk tempat entri berada. |
| [ShortName](../../aspose.zip.wim/wimentry/shortname/) { get; } | Mendapatkan nama pendek dari entri dalam gambar. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Extract](../../aspose.zip.wim/wimfileentry/extract/#extract_1)(Stream) | Mengekstrak entri ke aliran yang disediakan. |
| [Extract](../../aspose.zip.wim/wimfileentry/extract/#extract)(string) | Mengekstrak entri ke sistem file menggunakan jalur yang disediakan. |
| [Open](../../aspose.zip.wim/wimfileentry/open/)() | Membuka entri untuk ekstraksi dan menyediakan aliran dengan konten entri. |
| override [ToString](../../aspose.zip.wim/wimentry/tostring/)() |  |

### Lihat Juga

* class [WimEntry](../wimentry/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Wim](../../aspose.zip.wim/)
* assembly [Aspose.Zip](../../)


