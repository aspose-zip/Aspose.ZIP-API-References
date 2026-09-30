---
title: "Kelas CabArchive"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Kelas Aspose.Zip.Cab.CabArchive. Kelas ini mewakili file arsip CAB."
type: docs
weight: 310
url: /id/net/aspose.zip.cab/cabarchive/
---
## CabArchive class

Kelas ini mewakili file arsip CAB.

```csharp
public class CabArchive : IArchive
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [CabArchive](cabarchive/#constructor)(CabEntrySettings) | Menginisialisasi instance baru dari kelas `CabArchive` yang disiapkan untuk kompresi. |
| [CabArchive](cabarchive/#constructor_1)(Stream, CabLoadOptions) | Menginisialisasi sebuah instance baru dari kelas `CabArchive` dan menyusun daftar entri yang dapat diekstrak dari arsip. |
| [CabArchive](cabarchive/#constructor_2)(string, CabLoadOptions) | Menginisialisasi sebuah instance baru dari kelas `CabArchive` dan menyusun daftar entri yang dapat diekstrak dari arsip. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Entries](../../aspose.zip.cab/cabarchive/entries/) { get; } | Mendapatkan entri tipe [`CabEntry`](../cabentry/) yang membentuk arsip. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [CreateEntries](../../aspose.zip.cab/cabarchive/createentries/#createentries)(DirectoryInfo, bool) | Menambahkan semua file ke arsip, secara rekursif, dari direktori yang ditentukan. |
| [CreateEntries](../../aspose.zip.cab/cabarchive/createentries/#createentries_1)(string, bool) | Menambahkan semua file secara rekursif ke arsip dari jalur direktori yang ditentukan. |
| [CreateEntry](../../aspose.zip.cab/cabarchive/createentry/#createentry_1)(string, FileInfo, CabEntrySettings) | Buat satu entri dalam arsip. |
| [CreateEntry](../../aspose.zip.cab/cabarchive/createentry/#createentry)(string, Func&lt;Stream&gt;, CabEntrySettings) | Buat satu entri dalam arsip. |
| [CreateEntry](../../aspose.zip.cab/cabarchive/createentry/#createentry_2)(string, Stream, CabEntrySettings) | Buat satu entri dalam arsip. |
| [CreateEntry](../../aspose.zip.cab/cabarchive/createentry/#createentry_3)(string, string, CabEntrySettings) | Buat satu entri dalam arsip. |
| [Dispose](../../aspose.zip.cab/cabarchive/dispose/)() | Melakukan tugas yang ditentukan aplikasi terkait dengan membebaskan, melepaskan, atau mereset sumber daya yang tidak dikelola. |
| [ExtractToDirectory](../../aspose.zip.cab/cabarchive/extracttodirectory/)(string) | Mengekstrak semua file dalam arsip ke direktori yang disediakan. |
| [Save](../../aspose.zip.cab/cabarchive/save/#save)(Stream, CabSaveOptions) | Menyimpan arsip ke aliran yang disediakan. |
| [Save](../../aspose.zip.cab/cabarchive/save/#save_1)(string, CabSaveOptions) | Menyimpan arsip ke file tujuan yang disediakan. |

### Lihat Juga

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Cab](../../aspose.zip.cab/)
* assembly [Aspose.Zip](../../)


