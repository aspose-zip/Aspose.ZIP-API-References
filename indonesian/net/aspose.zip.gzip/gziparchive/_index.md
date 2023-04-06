---
title: Class GzipArchive
second_title: Aspose.ZIP untuk Referensi .NET API
description: Aspose.Zip.Gzip.GzipArchive kelas. Kelas ini mewakili file arsip gzip. Gunakan untuk menyusun atau mengekstrak arsip gzip.
type: docs
weight: 210
url: /id/net/aspose.zip.gzip/gziparchive/
---
## GzipArchive class

Kelas ini mewakili file arsip gzip. Gunakan untuk menyusun atau mengekstrak arsip gzip.

```csharp
public class GzipArchive : IArchive, IArchiveFileEntry
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [GzipArchive](gziparchive/#constructor)() | Menginisialisasi instance baru dari`GzipArchive` kelas disiapkan untuk mengompresi. |
| [GzipArchive](gziparchive/#constructor_1)(Stream, bool) | Menginisialisasi instance baru dari`GzipArchive` kelas disiapkan untuk dekompresi. |
| [GzipArchive](gziparchive/#constructor_2)(string, bool) | Menginisialisasi instance baru dari`GzipArchive` kelas. |

## Properti

| Nama | Keterangan |
| --- | --- |
| [Name](../../aspose.zip.gzip/gziparchive/name/) { get; } | Nama file asli. |

## Metode

| Nama | Keterangan |
| --- | --- |
| [Dispose](../../aspose.zip.gzip/gziparchive/dispose/)() | Melakukan tugas yang ditentukan aplikasi terkait dengan membebaskan, melepaskan, atau menyetel ulang sumber daya yang tidak dikelola. |
| [Extract](../../aspose.zip.gzip/gziparchive/extract/)(Stream) | Mengekstrak arsip ke aliran yang disediakan. |
| [Open](../../aspose.zip.gzip/gziparchive/open/)() | Membuka arsip untuk ekstraksi dan menyediakan aliran dengan konten arsip. |
| [Save](../../aspose.zip.gzip/gziparchive/save/#save)(Stream) | Menyimpan arsip ke aliran yang disediakan. |
| [Save](../../aspose.zip.gzip/gziparchive/save/#save_1)(string) | Menyimpan arsip ke file tujuan yang disediakan. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_1)(FileInfo) | Mengatur konten yang akan dikompresi dalam arsip. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_2)(Stream) | Mengatur konten yang akan dikompresi dalam arsip. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_3)(string) | Mengatur konten yang akan dikompresi dalam arsip. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource)(TarArchive) | Mengatur konten yang akan dikompresi dalam arsip. |

### Perkataan

Algoritma kompresi Gzip didasarkan pada algoritma DEFLATE, yang merupakan kombinasi dari pengkodean LZ77 dan Huffman.

### Lihat juga

* interface [IArchive](../../aspose.zip/iarchive/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* ruang nama [Aspose.Zip.Gzip](../../aspose.zip.gzip/)
* perakitan [Aspose.Zip](../../)


