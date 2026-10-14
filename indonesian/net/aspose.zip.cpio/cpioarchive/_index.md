---
title: "Kelas CpioArchive"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Aspose.Zip.Cpio.CpioArchive kelas. Kelas ini mewakili berkas arsip cpio"
type: docs
weight: 410
url: /id/net/aspose.zip.cpio/cpioarchive/
---
## CpioArchive class

Kelas ini mewakili file arsip cpio.

```csharp
public class CpioArchive : IArchive
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [CpioArchive](cpioarchive/#constructor)() | Menginisialisasi sebuah instance baru dari kelas `CpioArchive`. |
| [CpioArchive](cpioarchive/#constructor_1)(Stream) | Menginisialisasi sebuah instance baru dari kelas `CpioArchive` dan menyusun daftar entri yang dapat diekstrak dari arsip. |
| [CpioArchive](cpioarchive/#constructor_2)(string) | Menginisialisasi sebuah instance baru dari kelas `CpioArchive` dan menyusun daftar entri yang dapat diekstrak dari arsip. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Entries](../../aspose.zip.cpio/cpioarchive/entries/) { get; } | Mendapatkan entri tipe [`CpioEntry`](../cpioentry/) yang membentuk arsip. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [CreateEntries](../../aspose.zip.cpio/cpioarchive/createentries/#createentries)(DirectoryInfo, bool) | Menambahkan ke arsip semua file dan direktori secara rekursif dalam direktori yang diberikan. |
| [CreateEntries](../../aspose.zip.cpio/cpioarchive/createentries/#createentries_1)(string, bool) | Menambahkan ke arsip semua file dan direktori secara rekursif dalam direktori yang diberikan. |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry_1)(string, Stream) | Buat satu entri dalam arsip. |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry)(string, FileInfo, bool) | Buat satu entri dalam arsip. |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry_2)(string, string, bool) | Buat satu entri dalam arsip. |
| [DeleteEntry](../../aspose.zip.cpio/cpioarchive/deleteentry/#deleteentry)(CpioEntry) | Menghapus kemunculan pertama dari entri tertentu dalam daftar entri. |
| [DeleteEntry](../../aspose.zip.cpio/cpioarchive/deleteentry/#deleteentry_1)(int) | Menghapus entri dari daftar entri berdasarkan indeks. |
| [Dispose](../../aspose.zip.cpio/cpioarchive/dispose/)() | Melakukan tugas yang ditentukan aplikasi terkait dengan membebaskan, melepaskan, atau mereset sumber daya yang tidak dikelola. |
| [ExtractToDirectory](../../aspose.zip.cpio/cpioarchive/extracttodirectory/)(string) | Mengekstrak semua file dalam arsip ke direktori yang disediakan. |
| [Save](../../aspose.zip.cpio/cpioarchive/save/#save)(Stream, CpioFormat) | Menyimpan arsip ke aliran yang disediakan. |
| [Save](../../aspose.zip.cpio/cpioarchive/save/#save_1)(string, CpioFormat) | Menyimpan arsip ke file tujuan yang disediakan. |
| [SaveGzipped](../../aspose.zip.cpio/cpioarchive/savegzipped/#savegzipped)(Stream, CpioFormat) | Menyimpan arsip ke aliran dengan kompresi gzip. |
| [SaveGzipped](../../aspose.zip.cpio/cpioarchive/savegzipped/#savegzipped_1)(string, CpioFormat) | Menyimpan arsip ke file berdasarkan jalur dengan kompresi gzip. |
| [SaveLzipped](../../aspose.zip.cpio/cpioarchive/savelzipped/#savelzipped)(Stream, CpioFormat) | Menyimpan arsip ke aliran dengan kompresi lzip. |
| [SaveLzipped](../../aspose.zip.cpio/cpioarchive/savelzipped/#savelzipped_1)(string, CpioFormat) | Menyimpan arsip ke file berdasarkan jalur dengan kompresi lzip. |
| [SaveLZMACompressed](../../aspose.zip.cpio/cpioarchive/savelzmacompressed/#savelzmacompressed)(Stream, CpioFormat) | Menyimpan arsip ke aliran dengan kompresi LZMA. |
| [SaveLZMACompressed](../../aspose.zip.cpio/cpioarchive/savelzmacompressed/#savelzmacompressed_1)(string, CpioFormat) | Menyimpan arsip ke file berdasarkan jalur dengan kompresi lzma. |
| [SaveXzCompressed](../../aspose.zip.cpio/cpioarchive/savexzcompressed/#savexzcompressed)(Stream, CpioFormat, XzArchiveSettings) | Menyimpan arsip ke aliran dengan kompresi xz. |
| [SaveXzCompressed](../../aspose.zip.cpio/cpioarchive/savexzcompressed/#savexzcompressed_1)(string, CpioFormat, XzArchiveSettings) | Menyimpan arsip ke jalur berdasarkan jalur dengan kompresi xz. |
| [SaveZCompressed](../../aspose.zip.cpio/cpioarchive/savezcompressed/#savezcompressed)(Stream, CpioFormat) | Menyimpan arsip ke aliran dengan kompresi Z. |
| [SaveZCompressed](../../aspose.zip.cpio/cpioarchive/savezcompressed/#savezcompressed_1)(string, CpioFormat) | Menyimpan arsip ke jalur berdasarkan jalur dengan kompresi Z. |
| [SaveZstandard](../../aspose.zip.cpio/cpioarchive/savezstandard/#savezstandard)(Stream, CpioFormat) | Menyimpan arsip ke aliran dengan kompresi Zstandard. |
| [SaveZstandard](../../aspose.zip.cpio/cpioarchive/savezstandard/#savezstandard_1)(string, CpioFormat) | Menyimpan arsip ke file berdasarkan jalur dengan kompresi Zstandard. |

### Lihat Juga

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Cpio](../../aspose.zip.cpio/)
* assembly [Aspose.Zip](../../)


