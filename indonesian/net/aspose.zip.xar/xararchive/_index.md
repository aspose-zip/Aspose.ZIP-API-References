---
title: "Kelas XarArchive"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Kelas Aspose.Zip.Xar.XarArchive. Kelas ini mewakili file arsip xar"
type: docs
weight: 1420
url: /id/net/aspose.zip.xar/xararchive/
---
## XarArchive class

Kelas ini mewakili file arsip xar.

```csharp
public class XarArchive : IArchive
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [XarArchive](xararchive/#constructor)(XarCompressionSettings) | Menginisialisasi instance baru dari kelas `XarArchive`. |
| [XarArchive](xararchive/#constructor_1)(Stream, XarLoadOptions) | Menginisialisasi instance baru dari kelas `XarArchive` dan menyusun daftar entri yang dapat diekstrak dari arsip. |
| [XarArchive](xararchive/#constructor_2)(string, XarLoadOptions) | Menginisialisasi instance baru dari kelas `XarArchive` dan menyusun daftar entri yang dapat diekstrak dari arsip. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Entries](../../aspose.zip.xar/xararchive/entries/) { get; } | Mendapatkan entri tipe [`XarEntry`](../xarentry/) yang membentuk arsip. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [CreateEntries](../../aspose.zip.xar/xararchive/createentries/#createentries)(DirectoryInfo, bool, XarCompressionSettings) | Menambahkan ke arsip semua file dan direktori secara rekursif dalam direktori yang diberikan. |
| [CreateEntries](../../aspose.zip.xar/xararchive/createentries/#createentries_1)(string, bool, XarCompressionSettings) | Menambahkan ke arsip semua file dan direktori secara rekursif dalam direktori yang diberikan. |
| [CreateEntry](../../aspose.zip.xar/xararchive/createentry/#createentry_1)(string, Stream, XarCompressionSettings) | Buat satu entri dalam arsip. |
| [CreateEntry](../../aspose.zip.xar/xararchive/createentry/#createentry)(string, FileInfo, bool, XarCompressionSettings) | Buat satu entri dalam arsip. |
| [CreateEntry](../../aspose.zip.xar/xararchive/createentry/#createentry_2)(string, string, bool, XarCompressionSettings) | Buat satu entri dalam arsip. |
| [DeleteEntry](../../aspose.zip.xar/xararchive/deleteentry/)(XarEntry) | Menghapus kemunculan pertama dari entri tertentu dalam daftar entri. |
| [Dispose](../../aspose.zip.xar/xararchive/dispose/)() | Melakukan tugas yang ditentukan aplikasi terkait dengan membebaskan, melepaskan, atau mereset sumber daya yang tidak dikelola. |
| [ExtractToDirectory](../../aspose.zip.xar/xararchive/extracttodirectory/)(string) | Mengekstrak semua file dalam arsip ke direktori yang disediakan. |
| [Save](../../aspose.zip.xar/xararchive/save/#save)(Stream, XarSaveOptions) | Menyimpan arsip ke aliran yang disediakan. |
| [Save](../../aspose.zip.xar/xararchive/save/#save_1)(string, XarSaveOptions) | Menyimpan arsip ke file tujuan yang disediakan. |

### Lihat Juga

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Xar](../../aspose.zip.xar/)
* assembly [Aspose.Zip](../../)


