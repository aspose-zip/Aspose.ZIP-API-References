---
title: "Kelas GzipArchive"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Kelas Aspose.Zip.Gzip.GzipArchive. Kelas ini mewakili file arsip gzip. Gunakan untuk menyusun atau mengekstrak arsip gzip"
type: docs
weight: 510
url: /id/net/aspose.zip.gzip/gziparchive/
---
## GzipArchive class

Kelas ini mewakili file arsip gzip. Gunakan untuk membuat atau mengekstrak arsip gzip.

```csharp
public class GzipArchive : IArchive, IArchiveFileEntry
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [GzipArchive](gziparchive/#constructor)() | Menginisialisasi instance baru dari kelas `GzipArchive` yang disiapkan untuk kompresi. |
| [GzipArchive](gziparchive/#constructor_2)(Stream, bool) | Menginisialisasi instance baru dari kelas `GzipArchive` yang disiapkan untuk dekompresi. |
| [GzipArchive](gziparchive/#constructor_1)(Stream, GzipLoadOptions) | Menginisialisasi instance baru dari kelas `GzipArchive` yang disiapkan untuk dekompresi. |
| [GzipArchive](gziparchive/#constructor_4)(string, bool) | Menginisialisasi instance baru dari kelas `GzipArchive` yang disiapkan untuk dekompresi. |
| [GzipArchive](gziparchive/#constructor_3)(string, GzipLoadOptions) | Menginisialisasi instance baru dari kelas `GzipArchive` yang disiapkan untuk dekompresi. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Name](../../aspose.zip.gzip/gziparchive/name/) { get; } | Nama file asli. |
| [UncompressedSize](../../aspose.zip.gzip/gziparchive/uncompressedsize/) { get; } | Mendapatkan ukuran file asli. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Dispose](../../aspose.zip.gzip/gziparchive/dispose/)() | Melakukan tugas yang ditentukan aplikasi terkait dengan membebaskan, melepaskan, atau mereset sumber daya yang tidak dikelola. |
| [Extract](../../aspose.zip.gzip/gziparchive/extract/#extract_1)(Stream) | Mengekstrak arsip ke aliran yang disediakan. |
| [Extract](../../aspose.zip.gzip/gziparchive/extract/#extract)(string) | Mengekstrak arsip ke file berdasarkan jalur. |
| [ExtractToDirectory](../../aspose.zip.gzip/gziparchive/extracttodirectory/)(string) | Mengekstrak konten arsip ke direktori yang diberikan. |
| [Open](../../aspose.zip.gzip/gziparchive/open/)() | Membuka arsip untuk ekstraksi dan menyediakan aliran dengan konten arsip. |
| [Save](../../aspose.zip.gzip/gziparchive/save/#save)(Stream) | Menyimpan arsip ke aliran yang disediakan. |
| [Save](../../aspose.zip.gzip/gziparchive/save/#save_1)(string) | Menyimpan arsip ke file tujuan yang disediakan. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_1)(FileInfo) | Menetapkan konten yang akan dikompresi dalam arsip. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_2)(Stream) | Menetapkan konten yang akan dikompresi dalam arsip. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_3)(string) | Menetapkan konten yang akan dikompresi dalam arsip. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource)(TarArchive) | Menetapkan konten yang akan dikompresi dalam arsip. |

## Catatan

Algoritma kompresi Gzip didasarkan pada algoritma DEFLATE, yang merupakan kombinasi LZ77 dan pengkodean Huffman.

### Lihat Juga

* interface [IArchive](../../aspose.zip/iarchive/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Gzip](../../aspose.zip.gzip/)
* assembly [Aspose.Zip](../../)


