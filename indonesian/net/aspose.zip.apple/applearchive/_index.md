---
title: "Kelas AppleArchive"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Aspose.Zip.Apple.AppleArchive class. Kelas ini mewakili file Apple Archive .aar. Gunakan untuk menyusun file Apple Archive."
type: docs
weight: 60
url: /id/net/aspose.zip.apple/applearchive/
---
## AppleArchive class

Kelas ini mewakili file Apple Archive (.aar). Gunakan untuk menyusun file Apple Archive.

```csharp
public class AppleArchive : IArchive
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [AppleArchive](applearchive/#constructor)(AppleArchiveEntrySettings) | Menginisialisasi instance baru dari kelas `AppleArchive` dengan pengaturan yang digunakan untuk entri yang disusun. |
| [AppleArchive](applearchive/#constructor_1)(Stream, AppleArchiveLoadOptions) | Menginisialisasi instance baru dari kelas `AppleArchive` dan menyusun daftar entri yang dapat diekstrak dari arsip. |
| [AppleArchive](applearchive/#constructor_2)(string, AppleArchiveLoadOptions) | Menginisialisasi instance baru dari kelas `AppleArchive` dan menyusun daftar entri yang dapat diekstrak dari arsip. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Entries](../../aspose.zip.apple/applearchive/entries/) { get; } | Mendapatkan entri yang membentuk arsip. |
| [IsSolid](../../aspose.zip.apple/applearchive/issolid/) { get; } | Mendapatkan nilai yang menunjukkan apakah arsip menggunakan kompresi solid. Dalam mode solid, semua data entri dikompresi sebagai satu aliran dan ekstraksi entri individual tidak tersedia. Gunakan [`ExtractToDirectory`](../../aspose.zip/iarchive/extracttodirectory/) sebagai gantinya. |
| [NewEntrySettings](../../aspose.zip.apple/applearchive/newentrysettings/) { get; } | Mendapatkan pengaturan yang digunakan untuk entri yang baru disusun. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [CreateEntries](../../aspose.zip.apple/applearchive/createentries/)(DirectoryInfo, bool) | Menambahkan ke arsip semua file dan direktori secara rekursif dalam direktori yang diberikan. |
| [CreateEntry](../../aspose.zip.apple/applearchive/createentry/#createentry_1)(string, Stream) | Membuat satu entri di dalam arsip. |
| [CreateEntry](../../aspose.zip.apple/applearchive/createentry/#createentry)(string, FileInfo, bool) | Membuat satu entri di dalam arsip. |
| [CreateEntry](../../aspose.zip.apple/applearchive/createentry/#createentry_2)(string, string, bool) | Membuat satu entri di dalam arsip. |
| [Dispose](../../aspose.zip.apple/applearchive/dispose/)() | Melakukan tugas yang ditentukan aplikasi terkait dengan membebaskan, melepaskan, atau mereset sumber daya yang tidak dikelola. |
| [ExtractToDirectory](../../aspose.zip.apple/applearchive/extracttodirectory/)(string) | Mengekstrak semua file dalam arsip ke direktori yang disediakan. |
| [Save](../../aspose.zip.apple/applearchive/save/#save)(Stream) | Menyimpan arsip ke aliran yang disediakan. |
| [Save](../../aspose.zip.apple/applearchive/save/#save_1)(string) | Menyimpan arsip ke file tujuan yang disediakan. |

## Catatan

Apple dan Apple Archive adalah merek dagang Apple Inc.

### Lihat Juga

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Apple](../../aspose.zip.apple/)
* assembly [Aspose.Zip](../../)


