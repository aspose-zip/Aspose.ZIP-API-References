---
title: Class Archive
second_title: Aspose.ZIP untuk Referensi .NET API
description: Aspose.Zip.Archive kelas. Kelas ini mewakili file arsip zip. Gunakan untuk membuat mengekstrak atau memperbarui arsip zip.
type: docs
weight: 10
url: /id/net/aspose.zip/archive/
---
## Archive class

Kelas ini mewakili file arsip zip. Gunakan untuk membuat, mengekstrak, atau memperbarui arsip zip.

```csharp
public class Archive : IArchive
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [Archive](archive/#constructor)(ArchiveEntrySettings) | Menginisialisasi instance baru dari`Archive` kelas dengan pengaturan opsional untuk entri-entrinya. |
| [Archive](archive/#constructor_1)(Stream, ArchiveLoadOptions, ArchiveEntrySettings) | Menginisialisasi instance baru dari`Archive` kelas dan menulis daftar entri dapat diekstraksi dari arsip. |
| [Archive](archive/#constructor_2)(string, ArchiveLoadOptions, ArchiveEntrySettings) | Menginisialisasi instance baru dari`Archive` kelas dan menulis daftar entri dapat diekstraksi dari arsip. |

## Properti

| Nama | Keterangan |
| --- | --- |
| [Entries](../../aspose.zip/archive/entries/) { get; } | Mendapat entri dari[`ArchiveEntry`](../archiveentry/) ketik merupakan arsip. |
| [NewEntrySettings](../../aspose.zip/archive/newentrysettings/) { get; } | Pengaturan kompresi dan enkripsi digunakan untuk yang baru ditambahkan[`ArchiveEntry`](../archiveentry/) item. |

## Metode

| Nama | Keterangan |
| --- | --- |
| [CreateEntries](../../aspose.zip/archive/createentries/#createentries)(DirectoryInfo, bool) | Menambahkan ke arsip semua file dan direktori secara rekursif di direktori yang diberikan. |
| [CreateEntries](../../aspose.zip/archive/createentries/#createentries_1)(string, bool) | Menambahkan ke arsip semua file dan direktori secara rekursif di direktori yang diberikan. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_1)(string, Stream, ArchiveEntrySettings) | Buat satu entri dalam arsip. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry)(string, FileInfo, bool, ArchiveEntrySettings) | Buat satu entri dalam arsip. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_2)(string, Stream, ArchiveEntrySettings, FileSystemInfo) | Buat satu entri dalam arsip. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_3)(string, string, bool, ArchiveEntrySettings) | Buat satu entri dalam arsip. |
| [DeleteEntry](../../aspose.zip/archive/deleteentry/#deleteentry)(ArchiveEntry) | Menghapus kejadian pertama dari entri tertentu dari daftar entri. |
| [DeleteEntry](../../aspose.zip/archive/deleteentry/#deleteentry_1)(int) | Menghapus entri dari daftar entri menurut indeks. |
| [Dispose](../../aspose.zip/archive/dispose/)() | Melakukan tugas yang ditentukan aplikasi terkait dengan membebaskan, melepaskan, atau menyetel ulang sumber daya yang tidak dikelola. |
| [ExtractToDirectory](../../aspose.zip/archive/extracttodirectory/)(string) | Ekstrak semua file dalam arsip ke direktori yang disediakan. |
| [Save](../../aspose.zip/archive/save/#save)(Stream, ArchiveSaveOptions) | Menyimpan arsip ke aliran yang disediakan. |
| [Save](../../aspose.zip/archive/save/#save_1)(string, ArchiveSaveOptions) | Menyimpan arsip ke file tujuan yang disediakan. |
| [SaveSplit](../../aspose.zip/archive/savesplit/)(string, SplitArchiveSaveOptions) | Menyimpan arsip multi-volume ke direktori tujuan yang disediakan. |

### Lihat juga

* interface [IArchive](../iarchive/)
* ruang nama [Aspose.Zip](../../aspose.zip/)
* perakitan [Aspose.Zip](../../)


