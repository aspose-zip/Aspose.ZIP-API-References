---
title: "Kelas TarArchive"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Kelas Aspose.Zip.Tar.TarArchive. Kelas ini mewakili file arsip tar. Gunakan untuk membuat, mengekstrak, atau memperbarui arsip tar."
type: docs
weight: 1270
url: /id/net/aspose.zip.tar/tararchive/
---
## TarArchive class

Kelas ini mewakili file arsip tar. Gunakan untuk membuat, mengekstrak, atau memperbarui arsip tar.

```csharp
public class TarArchive : IArchive
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [TarArchive](tararchive/#constructor)() | Menginisialisasi instance baru dari kelas `TarArchive`. |
| [TarArchive](tararchive/#constructor_1)(Stream, TarLoadOptions) | Menginisialisasi instance baru dari kelas `TarArchive` dan menyusun daftar entri yang dapat diekstrak dari arsip. |
| [TarArchive](tararchive/#constructor_2)(string, TarLoadOptions) | Menginisialisasi instance baru dari kelas `TarArchive` dan menyusun daftar entri yang dapat diekstrak dari arsip. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Entries](../../aspose.zip.tar/tararchive/entries/) { get; } | Mendapatkan entri tipe [`TarEntry`](../tarentry/) yang membentuk arsip. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| static [FromGZip](../../aspose.zip.tar/tararchive/fromgzip/#fromgzip)(Stream) | Mengekstrak arsip gzip yang diberikan dan menyusun `TarArchive` dari data yang diekstrak. |
| static [FromGZip](../../aspose.zip.tar/tararchive/fromgzip/#fromgzip_1)(string) | Mengekstrak arsip gzip yang diberikan dan menyusun `TarArchive` dari data yang diekstrak. |
| static [FromLZ4](../../aspose.zip.tar/tararchive/fromlz4/#fromlz4)(Stream) | Mengekstrak arsip LZ4 yang diberikan dan menyusun `TarArchive` dari data yang diekstrak. |
| static [FromLZ4](../../aspose.zip.tar/tararchive/fromlz4/#fromlz4_1)(string) | Mengekstrak arsip LZ4 yang diberikan dan menyusun `TarArchive` dari data yang diekstrak. |
| static [FromLZip](../../aspose.zip.tar/tararchive/fromlzip/#fromlzip)(Stream) | Mengekstrak arsip lzip yang diberikan dan menyusun `TarArchive` dari data yang diekstrak. |
| static [FromLZip](../../aspose.zip.tar/tararchive/fromlzip/#fromlzip_1)(string) | Mengekstrak arsip lzip yang diberikan dan menyusun `TarArchive` dari data yang diekstrak. |
| static [FromLZMA](../../aspose.zip.tar/tararchive/fromlzma/#fromlzma)(Stream) | Mengekstrak arsip LZMA yang diberikan dan menyusun `TarArchive` dari data yang diekstrak. |
| static [FromLZMA](../../aspose.zip.tar/tararchive/fromlzma/#fromlzma_1)(string) | Mengekstrak arsip LZMA yang diberikan dan menyusun `TarArchive` dari data yang diekstrak. |
| static [FromXz](../../aspose.zip.tar/tararchive/fromxz/#fromxz)(Stream) | Mengekstrak arsip format xz yang diberikan dan menyusun `TarArchive` dari data yang diekstrak. |
| static [FromXz](../../aspose.zip.tar/tararchive/fromxz/#fromxz_1)(string) | Mengekstrak arsip format xz yang diberikan dan menyusun `TarArchive` dari data yang diekstrak. |
| static [FromZ](../../aspose.zip.tar/tararchive/fromz/#fromz)(Stream) | Mengekstrak arsip format Z yang diberikan dan menyusun `TarArchive` dari data yang diekstrak. |
| static [FromZ](../../aspose.zip.tar/tararchive/fromz/#fromz_1)(string) | Mengekstrak arsip format Z yang diberikan dan menyusun `TarArchive` dari data yang diekstrak. |
| static [FromZstandard](../../aspose.zip.tar/tararchive/fromzstandard/#fromzstandard)(Stream) | Mengekstrak arsip Zstandard yang diberikan dan menyusun `TarArchive` dari data yang diekstrak. |
| static [FromZstandard](../../aspose.zip.tar/tararchive/fromzstandard/#fromzstandard_1)(string) | Mengekstrak arsip Zstandard yang diberikan dan menyusun `TarArchive` dari data yang diekstrak. |
| [CreateEntries](../../aspose.zip.tar/tararchive/createentries/#createentries)(DirectoryInfo, bool) | Menambahkan ke arsip semua file dan direktori secara rekursif dalam direktori yang diberikan. |
| [CreateEntries](../../aspose.zip.tar/tararchive/createentries/#createentries_1)(string, bool) | Menambahkan ke arsip semua file dan direktori secara rekursif dalam direktori yang diberikan. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry/#createentry)(string, FileInfo, bool) | Buat satu entri dalam arsip. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry/#createentry_1)(string, Stream, FileSystemInfo) | Buat satu entri dalam arsip. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry/#createentry_2)(string, string, bool) | Buat satu entri dalam arsip. |
| [DeleteEntry](../../aspose.zip.tar/tararchive/deleteentry/#deleteentry_1)(int) | Menghapus entri dari daftar entri berdasarkan indeks. |
| [DeleteEntry](../../aspose.zip.tar/tararchive/deleteentry/#deleteentry)(TarEntry) | Menghapus kemunculan pertama dari entri tertentu dalam daftar entri. |
| [Dispose](../../aspose.zip.tar/tararchive/dispose/)() | Melakukan tugas yang ditentukan aplikasi terkait dengan membebaskan, melepaskan, atau mereset sumber daya yang tidak dikelola. |
| [ExtractToDirectory](../../aspose.zip.tar/tararchive/extracttodirectory/)(string) | Mengekstrak semua file dalam arsip ke direktori yang disediakan. |
| [Save](../../aspose.zip.tar/tararchive/save/#save)(Stream, TarFormat?) | Menyimpan arsip ke aliran yang disediakan. |
| [Save](../../aspose.zip.tar/tararchive/save/#save_1)(string, TarFormat?) | Menyimpan arsip ke file tujuan yang disediakan. |
| [SaveGzipped](../../aspose.zip.tar/tararchive/savegzipped/#savegzipped)(Stream, TarFormat?) | Menyimpan arsip ke aliran dengan kompresi gzip. |
| [SaveGzipped](../../aspose.zip.tar/tararchive/savegzipped/#savegzipped_1)(string, TarFormat?) | Menyimpan arsip ke file berdasarkan jalur dengan kompresi gzip. |
| [SaveLZ4Compressed](../../aspose.zip.tar/tararchive/savelz4compressed/#savelz4compressed)(Stream, TarFormat?) | Menyimpan arsip ke aliran dengan kompresi LZ4. |
| [SaveLZ4Compressed](../../aspose.zip.tar/tararchive/savelz4compressed/#savelz4compressed_1)(string, TarFormat?) | Menyimpan arsip ke file berdasarkan jalur dengan kompresi LZ4. |
| [SaveLzipped](../../aspose.zip.tar/tararchive/savelzipped/#savelzipped)(Stream, TarFormat?) | Menyimpan arsip ke aliran dengan kompresi lzip. |
| [SaveLzipped](../../aspose.zip.tar/tararchive/savelzipped/#savelzipped_1)(string, TarFormat?) | Menyimpan arsip ke file berdasarkan jalur dengan kompresi lzip. |
| [SaveLZMACompressed](../../aspose.zip.tar/tararchive/savelzmacompressed/#savelzmacompressed)(Stream, TarFormat?) | Menyimpan arsip ke aliran dengan kompresi LZMA. |
| [SaveLZMACompressed](../../aspose.zip.tar/tararchive/savelzmacompressed/#savelzmacompressed_1)(string, TarFormat?) | Menyimpan arsip ke file berdasarkan jalur dengan kompresi lzma. |
| [SaveXzCompressed](../../aspose.zip.tar/tararchive/savexzcompressed/#savexzcompressed)(Stream, TarFormat?, XzArchiveSettings) | Menyimpan arsip ke aliran dengan kompresi xz. |
| [SaveXzCompressed](../../aspose.zip.tar/tararchive/savexzcompressed/#savexzcompressed_1)(string, TarFormat?, XzArchiveSettings) | Menyimpan arsip ke jalur berdasarkan jalur dengan kompresi xz. |
| [SaveZCompressed](../../aspose.zip.tar/tararchive/savezcompressed/#savezcompressed)(Stream, TarFormat?) | Menyimpan arsip ke aliran dengan kompresi Z. |
| [SaveZCompressed](../../aspose.zip.tar/tararchive/savezcompressed/#savezcompressed_1)(string, TarFormat?) | Menyimpan arsip ke jalur berdasarkan jalur dengan kompresi Z. |
| [SaveZstandard](../../aspose.zip.tar/tararchive/savezstandard/#savezstandard)(Stream, TarFormat?) | Menyimpan arsip ke aliran dengan kompresi Zstandard. |
| [SaveZstandard](../../aspose.zip.tar/tararchive/savezstandard/#savezstandard_1)(string, TarFormat?) | Menyimpan arsip ke file berdasarkan jalur dengan kompresi Zstandard. |

### Lihat Juga

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Tar](../../aspose.zip.tar/)
* assembly [Aspose.Zip](../../)


