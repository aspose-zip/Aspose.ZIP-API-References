---
title: "Kelas AppleArchiveEntry"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Aspose.Zip.Apple.AppleArchiveEntry class. Mewakili entri sistem file di dalam AppleArchive"
type: docs
weight: 70
url: /id/net/aspose.zip.apple/applearchiveentry/
---
## AppleArchiveEntry class

Mewakili entri sistem file di dalam [`AppleArchive`](../applearchive/).

```csharp
public sealed class AppleArchiveEntry : IArchiveFileEntry
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [IsDirectory](../../aspose.zip.apple/applearchiveentry/isdirectory/) { get; } | Mendapatkan nilai yang menunjukkan apakah entri mewakili sebuah direktori. |
| [IsSymbolicLink](../../aspose.zip.apple/applearchiveentry/issymboliclink/) { get; } | Mendapatkan nilai yang menunjukkan apakah entri mewakili tautan simbolik. |
| [Length](../../aspose.zip.apple/applearchiveentry/length/) { get; } | Mendapatkan panjang tidak terkompresi entri dalam byte. |
| [Name](../../aspose.zip.apple/applearchiveentry/name/) { get; } | Mendapatkan jalur entri di dalam arsip. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Extract](../../aspose.zip.apple/applearchiveentry/extract/#extract_1)(Stream) | Mengekstrak entri ke aliran yang disediakan. |
| [Extract](../../aspose.zip.apple/applearchiveentry/extract/#extract)(string) | Mengekstrak entri ke sistem file menggunakan jalur yang disediakan. |
| [Open](../../aspose.zip.apple/applearchiveentry/open/)() | Membuka entri untuk ekstraksi dan menyediakan aliran dengan konten entri. |

## Catatan

Sebuah instance dari kelas ini dapat mewakili file biasa, direktori, atau tautan simbolik yang diurai dari Apple Archive yang ada, atau file atau direktori yang ditambahkan ke arsip yang sedang dibuat.

### Lihat Juga

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Apple](../../aspose.zip.apple/)
* assembly [Aspose.Zip](../../)


