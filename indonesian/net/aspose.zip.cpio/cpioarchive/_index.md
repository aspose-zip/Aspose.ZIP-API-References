---
title: Class CpioArchive
second_title: Aspose.ZIP untuk Referensi .NET API
description: Aspose.Zip.Cpio.CpioArchive kelas. Kelas ini mewakili file arsip cpio.
type: docs
weight: 160
url: /id/net/aspose.zip.cpio/cpioarchive/
---
## CpioArchive class

Kelas ini mewakili file arsip cpio.

```csharp
public class CpioArchive : IArchive
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [CpioArchive](cpioarchive/#constructor)() | Menginisialisasi instance baru dari`CpioArchive` kelas. |
| [CpioArchive](cpioarchive/#constructor_1)(Stream) | Menginisialisasi instance baru dari`CpioArchive` kelas dan menulis daftar entri dapat diekstraksi dari arsip. |
| [CpioArchive](cpioarchive/#constructor_2)(string) | Menginisialisasi instance baru dari`CpioArchive` kelas dan menulis daftar entri dapat diekstraksi dari arsip. |

## Properti

| Nama | Keterangan |
| --- | --- |
| [Entries](../../aspose.zip.cpio/cpioarchive/entries/) { get; } | Mendapat entri dari[`CpioEntry`](../cpioentry/) ketik merupakan arsip. |

## Metode

| Nama | Keterangan |
| --- | --- |
| [CreateEntries](../../aspose.zip.cpio/cpioarchive/createentries/#createentries)(DirectoryInfo, bool) | Menambahkan ke arsip semua file dan direktori secara rekursif di direktori yang diberikan. |
| [CreateEntries](../../aspose.zip.cpio/cpioarchive/createentries/#createentries_1)(string, bool) | Menambahkan ke arsip semua file dan direktori secara rekursif di direktori yang diberikan. |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry_1)(string, Stream) | Buat satu entri dalam arsip. |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry)(string, FileInfo, bool) | Buat satu entri dalam arsip. |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry_2)(string, string, bool) | Buat satu entri dalam arsip. |
| [DeleteEntry](../../aspose.zip.cpio/cpioarchive/deleteentry/#deleteentry)(CpioEntry) | Menghapus kejadian pertama dari entri tertentu dari daftar entri. |
| [DeleteEntry](../../aspose.zip.cpio/cpioarchive/deleteentry/#deleteentry_1)(int) | Menghapus entri dari daftar entri menurut indeks. |
| [Dispose](../../aspose.zip.cpio/cpioarchive/dispose/)() | Melakukan tugas yang ditentukan aplikasi terkait dengan membebaskan, melepaskan, atau menyetel ulang sumber daya yang tidak dikelola. |
| [ExtractToDirectory](../../aspose.zip.cpio/cpioarchive/extracttodirectory/)(string) | Ekstrak semua file dalam arsip ke direktori yang disediakan. |
| [Save](../../aspose.zip.cpio/cpioarchive/save/#save)(Stream, CpioFormat) | Menyimpan arsip ke aliran yang disediakan. |
| [Save](../../aspose.zip.cpio/cpioarchive/save/#save_1)(string, CpioFormat) | Menyimpan arsip ke file tujuan yang disediakan. |
| [SaveGzipped](../../aspose.zip.cpio/cpioarchive/savegzipped/#savegzipped)(Stream, CpioFormat) | Menyimpan arsip ke aliran dengan kompresi gzip. |
| [SaveGzipped](../../aspose.zip.cpio/cpioarchive/savegzipped/#savegzipped_1)(string, CpioFormat) | Menyimpan arsip ke file dengan jalur dengan kompresi gzip. |
| [SaveXzCompressed](../../aspose.zip.cpio/cpioarchive/savexzcompressed/#savexzcompressed)(Stream, CpioFormat, XzArchiveSettings) | Menyimpan arsip ke aliran dengan kompresi xz. |
| [SaveXzCompressed](../../aspose.zip.cpio/cpioarchive/savexzcompressed/#savexzcompressed_1)(string, CpioFormat, XzArchiveSettings) | Menyimpan arsip ke jalur demi jalur dengan kompresi xz. |

### Lihat juga

* interface [IArchive](../../aspose.zip/iarchive/)
* ruang nama [Aspose.Zip.Cpio](../../aspose.zip.cpio/)
* perakitan [Aspose.Zip](../../)


