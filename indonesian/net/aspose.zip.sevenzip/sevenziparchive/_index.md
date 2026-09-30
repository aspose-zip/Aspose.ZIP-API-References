---
title: "Kelas SevenZipArchive"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Kelas Aspose.Zip.SevenZip.SevenZipArchive. Kelas ini mewakili file arsip 7z. Gunakan untuk menyusun dan mengekstrak arsip 7z."
type: docs
weight: 1190
url: /id/net/aspose.zip.sevenzip/sevenziparchive/
---
## SevenZipArchive class

Kelas ini mewakili file arsip 7z. Gunakan untuk membuat dan mengekstrak arsip 7z.

```csharp
public class SevenZipArchive : IArchive
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [SevenZipArchive](sevenziparchive/#constructor)(SevenZipEntrySettings) | Menginisialisasi instance baru dari kelas `SevenZipArchive` dengan pengaturan opsional untuk entri-entrinya. |
| [SevenZipArchive](sevenziparchive/#constructor_1)(Stream, SevenZipLoadOptions) | Menginisialisasi instance baru dari kelas `SevenZipArchive` dan menyusun daftar entri yang dapat diekstrak dari arsip. |
| [SevenZipArchive](sevenziparchive/#constructor_2)(Stream, string) | Menginisialisasi instance baru dari kelas `SevenZipArchive` dan menyusun daftar entri yang dapat diekstrak dari arsip. |
| [SevenZipArchive](sevenziparchive/#constructor_3)(string, SevenZipLoadOptions) | Menginisialisasi instance baru dari kelas `SevenZipArchive` dan menyusun daftar entri yang dapat diekstrak dari arsip. |
| [SevenZipArchive](sevenziparchive/#constructor_4)(string, string) | Menginisialisasi instance baru dari kelas `SevenZipArchive` dan menyusun daftar entri yang dapat diekstrak dari arsip. |
| [SevenZipArchive](sevenziparchive/#constructor_5)(string[], string) | Menginisialisasi instance baru dari kelas `SevenZipArchive` dari arsip 7z multi-volume dan menyusun daftar entri yang dapat diekstrak dari arsip. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Entries](../../aspose.zip.sevenzip/sevenziparchive/entries/) { get; } | Mendapatkan entri tipe [`SevenZipArchiveEntry`](../sevenziparchiveentry/) yang membentuk arsip. |
| [NewEntrySettings](../../aspose.zip.sevenzip/sevenziparchive/newentrysettings/) { get; } | Pengaturan kompresi dan enkripsi yang digunakan untuk item [`SevenZipArchiveEntry`](../sevenziparchiveentry/) yang baru ditambahkan. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [CreateEntries](../../aspose.zip.sevenzip/sevenziparchive/createentries/#createentries)(DirectoryInfo, bool) | Menambahkan ke arsip semua file dan direktori secara rekursif dalam direktori yang diberikan. |
| [CreateEntries](../../aspose.zip.sevenzip/sevenziparchive/createentries/#createentries_1)(string, bool) | Menambahkan ke arsip semua file dan direktori secara rekursif dalam direktori yang diberikan. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry)(string, Func&lt;Stream&gt;, SevenZipEntrySettings) | Buat satu entri dalam arsip. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_2)(string, Stream, SevenZipEntrySettings) | Buat satu entri dalam arsip. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_1)(string, FileInfo, bool, SevenZipEntrySettings) | Buat satu entri dalam arsip. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_3)(string, Stream, SevenZipEntrySettings, FileSystemInfo) | Buat satu entri dalam arsip. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_4)(string, string, bool, SevenZipEntrySettings) | Buat satu entri dalam arsip. |
| [Dispose](../../aspose.zip.sevenzip/sevenziparchive/dispose/)() | Melakukan tugas yang ditentukan aplikasi terkait dengan membebaskan, melepaskan, atau mereset sumber daya yang tidak dikelola. |
| [ExtractToDirectory](../../aspose.zip.sevenzip/sevenziparchive/extracttodirectory/)(string, string) | Mengekstrak semua file dalam arsip ke direktori yang disediakan. |
| [Save](../../aspose.zip.sevenzip/sevenziparchive/save/#save)(Stream, SevenZipArchiveSaveOptions) | Menyimpan arsip 7z ke aliran yang disediakan. |
| [Save](../../aspose.zip.sevenzip/sevenziparchive/save/#save_1)(string, SevenZipArchiveSaveOptions) | Menyimpan arsip ke file tujuan yang disediakan. |
| [SaveSplit](../../aspose.zip.sevenzip/sevenziparchive/savesplit/)(string, SplitSevenZipArchiveSaveOptions) | Menyimpan arsip multi-volume ke direktori tujuan yang disediakan. |

### Lihat Juga

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.SevenZip](../../aspose.zip.sevenzip/)
* assembly [Aspose.Zip](../../)


