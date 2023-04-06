---
title: Class WimFileEntry
second_title: Aspose.ZIP untuk Referensi .NET API
description: Aspose.Zip.Wim.WimFileEntry kelas. Merupakan file tunggal dalam arsip wim.
type: docs
weight: 790
url: /id/net/aspose.zip.wim/wimfileentry/
---
## WimFileEntry class

Merupakan file tunggal dalam arsip wim.

```csharp
public sealed class WimFileEntry : WimEntry, IArchiveFileEntry
```

## Properti

| Nama | Keterangan |
| --- | --- |
| [AlternateDataStreams](../../aspose.zip.wim/wimentry/alternatedatastreams/) { get; } | Mendapatkan nama aliran data alternatif untuk file atau direktori. |
| [Archive](../../aspose.zip.wim/wimentry/archive/) { get; } | Mendapatkan arsip tempat entri tersebut berada. |
| [ChangeTime](../../aspose.zip.wim/wimentry/changetime/) { get; } | Mendapatkan terakhir kali file atau direktori diubah. |
| [CreationTime](../../aspose.zip.wim/wimentry/creationtime/) { get; } | Mendapatkan waktu pembuatan file atau direktori. |
| [FileAttributes](../../aspose.zip.wim/wimentry/fileattributes/) { get; } | Mendapat atribut file atau direktori. |
| [FullPath](../../aspose.zip.wim/wimentry/fullpath/) { get; } | Mendapat jalur lengkap dari entri di dalam gambar. |
| [HardLink](../../aspose.zip.wim/wimentry/hardlink/) { get; } | Mendapatkan id hardlink dari file atau direktori. |
| [HasHardLinks](../../aspose.zip.wim/wimentry/hashardlinks/) { get; } | Mendapat apakah file atau direktori dikenal dengan nama lain. |
| [Image](../../aspose.zip.wim/wimentry/image/) { get; } | Mendapat gambar milik entri tersebut. |
| [IsDirectory](../../aspose.zip.wim/wimentry/isdirectory/) { get; } | Mendapat nilai yang menunjukkan apakah entri mewakili direktori. |
| [LastAccessTime](../../aspose.zip.wim/wimentry/lastaccesstime/) { get; } | Mendapat waktu akses terakhir dari file atau direktori. |
| [LastWriteTime](../../aspose.zip.wim/wimentry/lastwritetime/) { get; } | Mendapatkan waktu modifikasi file atau direktori. |
| [Length](../../aspose.zip.wim/wimfileentry/length/) { get; } | Mendapatkan panjang entri dalam byte. |
| [Name](../../aspose.zip.wim/wimentry/name/) { get; } | Mendapat nama entri dalam gambar. |
| [Parent](../../aspose.zip.wim/wimentry/parent/) { get; } | Mendapatkan direktori induk tempat entri tersebut berada. |
| [ShortName](../../aspose.zip.wim/wimentry/shortname/) { get; } | Mendapat nama pendek entri dalam gambar. |

## Metode

| Nama | Keterangan |
| --- | --- |
| [Extract](../../aspose.zip.wim/wimfileentry/extract/#extract_1)(Stream) | Mengekstrak entri ke aliran yang disediakan. |
| [Extract](../../aspose.zip.wim/wimfileentry/extract/#extract)(string) | Mengekstrak entri ke sistem file dengan jalur yang disediakan. |
| [Open](../../aspose.zip.wim/wimfileentry/open/)() | Membuka entri untuk ekstraksi dan menyediakan aliran dengan konten entri. |
| override [ToString](../../aspose.zip.wim/wimentry/tostring/)() |  |

### Lihat juga

* class [WimEntry](../wimentry/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* ruang nama [Aspose.Zip.Wim](../../aspose.zip.wim/)
* perakitan [Aspose.Zip](../../)


