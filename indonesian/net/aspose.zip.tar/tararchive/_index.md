---
title: Class TarArchive
second_title: Aspose.ZIP untuk Referensi .NET API
description: Aspose.Zip.Tar.TarArchive kelas. Kelas ini mewakili file arsip tar. Gunakan untuk menyusun mengekstrak atau memperbarui arsip tar.
type: docs
weight: 730
url: /id/net/aspose.zip.tar/tararchive/
---
## TarArchive class

Kelas ini mewakili file arsip tar. Gunakan untuk menyusun, mengekstrak, atau memperbarui arsip tar.

```csharp
public class TarArchive : IArchive
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [TarArchive](tararchive/#constructor)() | Menginisialisasi instance baru dari`TarArchive` kelas. |
| [TarArchive](tararchive/#constructor_1)(Stream) | Menginisialisasi instance baru dari[`Archive`](../../aspose.zip/archive/) kelas dan menulis daftar entri dapat diekstraksi dari arsip. |
| [TarArchive](tararchive/#constructor_2)(string) | Menginisialisasi instance baru dari`TarArchive` kelas dan menulis daftar entri dapat diekstraksi dari arsip. |

## Properti

| Nama | Keterangan |
| --- | --- |
| [Entries](../../aspose.zip.tar/tararchive/entries/) { get; } | Mendapat entri dari[`TarEntry`](../tarentry/) ketik merupakan arsip. |

## Metode

| Nama | Keterangan |
| --- | --- |
| static [FromGZip](../../aspose.zip.tar/tararchive/fromgzip/#fromgzip)(Stream) | Mengekstrak arsip dan komposisi gzip yang disediakan`TarArchive` dari data yang diekstraksi. |
| static [FromGZip](../../aspose.zip.tar/tararchive/fromgzip/#fromgzip_1)(string) | Mengekstrak arsip dan komposisi gzip yang disediakan`TarArchive` dari data yang diekstraksi. |
| static [FromLZip](../../aspose.zip.tar/tararchive/fromlzip/#fromlzip)(Stream) | Ekstrak yang disediakan arsip dan penulisan lzip`TarArchive` dari data yang diekstraksi. |
| static [FromLZip](../../aspose.zip.tar/tararchive/fromlzip/#fromlzip_1)(string) | Ekstrak yang disediakan arsip dan penulisan lzip`TarArchive` dari data yang diekstraksi. |
| static [FromXz](../../aspose.zip.tar/tararchive/fromxz/#fromxz)(Stream) | Ekstrak arsip dan penulisan format xz yang disediakan`TarArchive` dari data yang diekstraksi. |
| static [FromXz](../../aspose.zip.tar/tararchive/fromxz/#fromxz_1)(string) | Ekstrak arsip dan penulisan format xz yang disediakan`TarArchive` dari data yang diekstraksi. |
| static [FromZ](../../aspose.zip.tar/tararchive/fromz/#fromz)(Stream) | Ekstrak disediakan arsip dan komposisi format Z`TarArchive` dari data yang diekstraksi. |
| static [FromZ](../../aspose.zip.tar/tararchive/fromz/#fromz_1)(string) | Ekstrak disediakan arsip dan komposisi format Z`TarArchive` dari data yang diekstraksi. |
| [CreateEntries](../../aspose.zip.tar/tararchive/createentries/#createentries)(DirectoryInfo, bool) | Menambahkan ke arsip semua file dan direktori secara rekursif di direktori yang diberikan. |
| [CreateEntries](../../aspose.zip.tar/tararchive/createentries/#createentries_1)(string, bool) | Menambahkan ke arsip semua file dan direktori secara rekursif di direktori yang diberikan. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry/#createentry)(string, FileInfo, bool) | Buat satu entri dalam arsip. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry/#createentry_1)(string, Stream, FileSystemInfo) | Buat satu entri dalam arsip. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry/#createentry_2)(string, string, bool) | Buat satu entri dalam arsip. |
| [DeleteEntry](../../aspose.zip.tar/tararchive/deleteentry/#deleteentry_1)(int) | Menghapus entri dari daftar entri menurut indeks. |
| [DeleteEntry](../../aspose.zip.tar/tararchive/deleteentry/#deleteentry)(TarEntry) | Menghapus kejadian pertama dari entri tertentu dari daftar entri. |
| [Dispose](../../aspose.zip.tar/tararchive/dispose/)() | Melakukan tugas yang ditentukan aplikasi terkait dengan membebaskan, melepaskan, atau menyetel ulang sumber daya yang tidak dikelola. |
| [ExtractToDirectory](../../aspose.zip.tar/tararchive/extracttodirectory/)(string) | Ekstrak semua file dalam arsip ke direktori yang disediakan. |
| [Save](../../aspose.zip.tar/tararchive/save/#save)(Stream, TarFormat?) | Menyimpan arsip ke aliran yang disediakan. |
| [Save](../../aspose.zip.tar/tararchive/save/#save_1)(string, TarFormat?) | Menyimpan arsip ke file tujuan yang disediakan. |
| [SaveGzipped](../../aspose.zip.tar/tararchive/savegzipped/#savegzipped)(Stream, TarFormat?) | Menyimpan arsip ke aliran dengan kompresi gzip. |
| [SaveGzipped](../../aspose.zip.tar/tararchive/savegzipped/#savegzipped_1)(string, TarFormat?) | Menyimpan arsip ke file dengan jalur dengan kompresi gzip. |
| [SaveLzipped](../../aspose.zip.tar/tararchive/savelzipped/#savelzipped)(Stream, TarFormat?) | Menyimpan arsip ke aliran dengan kompresi lzip. |
| [SaveLzipped](../../aspose.zip.tar/tararchive/savelzipped/#savelzipped_1)(string, TarFormat?) | Menyimpan arsip ke file dengan jalur dengan kompresi lzip. |
| [SaveXzCompressed](../../aspose.zip.tar/tararchive/savexzcompressed/#savexzcompressed)(Stream, TarFormat?, XzArchiveSettings) | Menyimpan arsip ke aliran dengan kompresi xz. |
| [SaveXzCompressed](../../aspose.zip.tar/tararchive/savexzcompressed/#savexzcompressed_1)(string, TarFormat?, XzArchiveSettings) | Menyimpan arsip ke jalur demi jalur dengan kompresi xz. |
| [SaveZCompressed](../../aspose.zip.tar/tararchive/savezcompressed/#savezcompressed)(Stream, TarFormat?) | Menyimpan arsip ke aliran dengan kompresi Z. |
| [SaveZCompressed](../../aspose.zip.tar/tararchive/savezcompressed/#savezcompressed_1)(string, TarFormat?) | Menyimpan arsip ke jalur demi jalur dengan kompresi Z. |

### Lihat juga

* interface [IArchive](../../aspose.zip/iarchive/)
* ruang nama [Aspose.Zip.Tar](../../aspose.zip.tar/)
* perakitan [Aspose.Zip](../../)


