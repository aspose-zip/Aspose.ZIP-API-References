---
title: Class SevenZipArchive
second_title: Aspose.ZIP untuk Referensi .NET API
description: Aspose.Zip.SevenZip.SevenZipArchive kelas. Kelas ini mewakili file arsip 7z. Gunakan untuk menyusun dan mengekstrak arsip 7z.
type: docs
weight: 660
url: /id/net/aspose.zip.sevenzip/sevenziparchive/
---
## SevenZipArchive class

Kelas ini mewakili file arsip 7z. Gunakan untuk menyusun dan mengekstrak arsip 7z.

```csharp
public class SevenZipArchive : IArchive
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [SevenZipArchive](sevenziparchive/#constructor)(SevenZipEntrySettings) | Menginisialisasi instance baru dari`SevenZipArchive` kelas dengan pengaturan opsional untuk entri-entrinya. |
| [SevenZipArchive](sevenziparchive/#constructor_1)(Stream) | Menginisialisasi instance baru dari`SevenZipArchive` kelas dan menulis daftar entri dapat diekstraksi dari arsip. |
| [SevenZipArchive](sevenziparchive/#constructor_2)(string) | Menginisialisasi instance baru dari`SevenZipArchive` kelas dan menulis daftar entri dapat diekstraksi dari arsip. |

## Properti

| Nama | Keterangan |
| --- | --- |
| [Entries](../../aspose.zip.sevenzip/sevenziparchive/entries/) { get; } | Mendapat entri dari[`SevenZipArchiveEntry`](../sevenziparchiveentry/) ketik merupakan arsip. |
| [NewEntrySettings](../../aspose.zip.sevenzip/sevenziparchive/newentrysettings/) { get; } | Pengaturan kompresi dan enkripsi digunakan untuk yang baru ditambahkan[`SevenZipArchiveEntry`](../sevenziparchiveentry/) item. |

## Metode

| Nama | Keterangan |
| --- | --- |
| [CreateEntries](../../aspose.zip.sevenzip/sevenziparchive/createentries/#createentries)(DirectoryInfo, bool) | Menambahkan ke arsip semua file dan direktori secara rekursif di direktori yang diberikan. |
| [CreateEntries](../../aspose.zip.sevenzip/sevenziparchive/createentries/#createentries_1)(string, bool) | Menambahkan ke arsip semua file dan direktori secara rekursif di direktori yang diberikan. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_1)(string, Stream, SevenZipEntrySettings) | Buat satu entri dalam arsip. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry)(string, FileInfo, bool, SevenZipEntrySettings) | Buat satu entri dalam arsip. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_2)(string, Stream, SevenZipEntrySettings, FileSystemInfo) | Buat satu entri dalam arsip. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_3)(string, string, bool, SevenZipEntrySettings) | Buat satu entri dalam arsip. |
| [Dispose](../../aspose.zip.sevenzip/sevenziparchive/dispose/)() | Melakukan tugas yang ditentukan aplikasi terkait dengan membebaskan, melepaskan, atau menyetel ulang sumber daya yang tidak dikelola. |
| [ExtractToDirectory](../../aspose.zip.sevenzip/sevenziparchive/extracttodirectory/)(string, string) | Ekstrak semua file dalam arsip ke direktori yang disediakan. |
| [Save](../../aspose.zip.sevenzip/sevenziparchive/save/#save)(Stream) | Menyimpan arsip 7z ke aliran yang disediakan. |
| [Save](../../aspose.zip.sevenzip/sevenziparchive/save/#save_1)(string) | Menyimpan arsip ke file tujuan yang disediakan. |
| [SaveSplit](../../aspose.zip.sevenzip/sevenziparchive/savesplit/)(string, SplitSevenZipArchiveSaveOptions) | Menyimpan arsip multi-volume ke direktori tujuan yang disediakan. |

### Lihat juga

* interface [IArchive](../../aspose.zip/iarchive/)
* ruang nama [Aspose.Zip.SevenZip](../../aspose.zip.sevenzip/)
* perakitan [Aspose.Zip](../../)


