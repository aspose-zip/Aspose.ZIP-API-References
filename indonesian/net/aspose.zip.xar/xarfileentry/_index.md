---
title: Class XarFileEntry
second_title: Aspose.ZIP untuk Referensi .NET API
description: Aspose.Zip.Xar.XarFileEntry kelas. Merupakan entri file dalam arsip xar.
type: docs
weight: 840
url: /id/net/aspose.zip.xar/xarfileentry/
---
## XarFileEntry class

Merupakan entri file dalam arsip xar.

```csharp
public abstract class XarFileEntry : XarEntry, IArchiveFileEntry
```

## Properti

| Nama | Keterangan |
| --- | --- |
| [CreationTime](../../aspose.zip.xar/xarentry/creationtime/) { get; } | Mendapatkan waktu pembuatan file atau direktori. |
| [FullPath](../../aspose.zip.xar/xarentry/fullpath/) { get; } | Mendapat path lengkap dari entri di dalam arsip. |
| [IsDirectory](../../aspose.zip.xar/xarentry/isdirectory/) { get; } | Mendapat nilai yang menunjukkan apakah entri mewakili direktori. |
| [LastAccessTime](../../aspose.zip.xar/xarentry/lastaccesstime/) { get; } | Mendapat waktu akses terakhir dari file atau direktori. |
| [LastWriteTime](../../aspose.zip.xar/xarentry/lastwritetime/) { get; } | Mendapatkan waktu modifikasi file atau direktori. |
| abstract [Length](../../aspose.zip.xar/xarfileentry/length/) { get; } | Mendapatkan panjang entri dalam byte. |
| [Name](../../aspose.zip.xar/xarentry/name/) { get; } | Mendapat nama entri dalam arsip. |
| [Parent](../../aspose.zip.xar/xarentry/parent/) { get; } | Mendapatkan direktori induk tempat entri tersebut berada. |

## Metode

| Nama | Keterangan |
| --- | --- |
| abstract [Extract](../../aspose.zip.xar/xarfileentry/extract/#extract_1)(Stream) | Mengekstrak entri ke aliran yang disediakan. |
| abstract [Extract](../../aspose.zip.xar/xarfileentry/extract/#extract)(string) | Mengekstrak entri ke sistem file dengan jalur yang disediakan. |
| abstract [Open](../../aspose.zip.xar/xarfileentry/open/)() | Membuka entri untuk ekstraksi dan menyediakan aliran dengan konten entri. |
| override [ToString](../../aspose.zip.xar/xarentry/tostring/)() |  |

### Lihat juga

* class [XarEntry](../xarentry/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* ruang nama [Aspose.Zip.Xar](../../aspose.zip.xar/)
* perakitan [Aspose.Zip](../../)


