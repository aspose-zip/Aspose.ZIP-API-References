---
title: "Kelas AlzEntry"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Kelas Aspose.Zip.Alz.AlzEntry. Mewakili entri file dalam arsip ALZ dengan semua metadata-nya"
type: docs
weight: 30
url: /id/net/aspose.zip.alz/alzentry/
---
## AlzEntry class

Mewakili entri file dalam arsip ALZ dengan semua metadata-nya.

```csharp
public abstract class AlzEntry : IArchiveFileEntry
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [CompressedSize](../../aspose.zip.alz/alzentry/compressedsize/) { get; } | Ukuran terkompresi data file dalam byte. |
| [IsDirectory](../../aspose.zip.alz/alzentry/isdirectory/) { get; } | Mengembalikan true jika entri ini mewakili sebuah direktori. |
| [Length](../../aspose.zip.alz/alzentry/length/) { get; } |  |
| [Name](../../aspose.zip.alz/alzentry/name/) { get; } | Nama file (tanpa jalur). |
| [UncompressedSize](../../aspose.zip.alz/alzentry/uncompressedsize/) { get; } | Ukuran data file yang tidak terkompresi dalam byte. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Extract](../../aspose.zip.alz/alzentry/extract/#extract_1)(Stream, string) | Mengekstrak entri ke aliran yang disediakan. |
| [Extract](../../aspose.zip.alz/alzentry/extract/#extract)(string, string) | Mengekstrak entri ke sistem file menggunakan jalur yang disediakan. |
| [Open](../../aspose.zip.alz/alzentry/open/)(string) | Membuka entri untuk ekstraksi dan menyediakan aliran dengan konten entri yang didekompresi. |

### Lihat Juga

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Alz](../../aspose.zip.alz/)
* assembly [Aspose.Zip](../../)


