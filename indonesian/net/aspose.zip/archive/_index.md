---
title: "Kelas Archive"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Kelas Aspose.Zip.Archive. Kelas ini mewakili file arsip zip. Gunakan untuk menyusun, mengekstrak, atau memperbarui arsip zip"
type: docs
weight: 160
url: /id/net/aspose.zip/archive/
---
## Archive class

Kelas ini mewakili file arsip zip. Gunakan untuk menyusun, mengekstrak, atau memperbarui arsip zip.

```csharp
public class Archive : IArchive
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [Archive](archive/#constructor)(ArchiveEntrySettings) | Menginisialisasi instance baru dari kelas `Archive` dengan pengaturan opsional untuk entri-entrinya. |
| [Archive](archive/#constructor_1)(Stream, ArchiveLoadOptions, ArchiveEntrySettings) | Menginisialisasi instance baru dari kelas `Archive` dan menyusun daftar entri yang dapat diekstrak dari arsip. |
| [Archive](archive/#constructor_2)(string, ArchiveLoadOptions, ArchiveEntrySettings) | Menginisialisasi instance baru dari kelas `Archive` dan menyusun daftar entri yang dapat diekstrak dari arsip. |
| [Archive](archive/#constructor_3)(string, string[], ArchiveLoadOptions) | Menginisialisasi instance baru dari kelas `Archive` dari arsip ZIP multi-volume dan menyusun daftar entri yang dapat diekstrak dari arsip. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Comment](../../aspose.zip/archive/comment/) { get; } | Mendapatkan komentar untuk seluruh arsip. |
| [Entries](../../aspose.zip/archive/entries/) { get; } | Mendapatkan entri berjenis [`ArchiveEntry`](../archiveentry/) yang membentuk arsip. |
| [NewEntrySettings](../../aspose.zip/archive/newentrysettings/) { get; } | Pengaturan kompresi dan enkripsi yang digunakan untuk item [`ArchiveEntry`](../archiveentry/) yang baru ditambahkan. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [CreateEntries](../../aspose.zip/archive/createentries/#createentries)(DirectoryInfo, bool) | Tambahkan ke arsip semua file dan direktori secara rekursif dalam direktori yang diberikan. |
| [CreateEntries](../../aspose.zip/archive/createentries/#createentries_1)(string, bool) | Tambahkan ke arsip semua file dan direktori secara rekursif dalam direktori yang diberikan. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry)(string, Func&lt;Stream&gt;, ArchiveEntrySettings) | Buat satu entri dalam arsip. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_2)(string, Stream, ArchiveEntrySettings) | Buat satu entri dalam arsip. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_1)(string, FileInfo, bool, ArchiveEntrySettings) | Buat satu entri dalam arsip. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_3)(string, Stream, ArchiveEntrySettings, FileSystemInfo) | Buat satu entri dalam arsip. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_4)(string, string, bool, ArchiveEntrySettings) | Buat satu entri dalam arsip. |
| [DeleteEntry](../../aspose.zip/archive/deleteentry/#deleteentry)(ArchiveEntry) | Menghapus kemunculan pertama dari entri spesifik dari daftar entri. |
| [DeleteEntry](../../aspose.zip/archive/deleteentry/#deleteentry_1)(int) | Menghapus entri dari daftar entri berdasarkan indeks. |
| [Dispose](../../aspose.zip/archive/dispose/)() | Melakukan tugas yang ditentukan aplikasi terkait dengan membebaskan, melepaskan, atau mereset sumber daya yang tidak dikelola. |
| [ExtractToDirectory](../../aspose.zip/archive/extracttodirectory/)(string) | Mengekstrak semua file dalam arsip ke direktori yang disediakan. |
| [Save](../../aspose.zip/archive/save/#save)(Stream, ArchiveSaveOptions) | Menyimpan arsip ke aliran yang disediakan. |
| [Save](../../aspose.zip/archive/save/#save_1)(string, ArchiveSaveOptions) | Menyimpan arsip ke file tujuan yang disediakan. |
| [SaveSplit](../../aspose.zip/archive/savesplit/#savesplit)(IVolumeStreamProvider, SplitArchiveSaveOptions) | Menyimpan arsip multi-volume ke aliran yang disediakan oleh penyedia volume. |
| [SaveSplit](../../aspose.zip/archive/savesplit/#savesplit_1)(string, SplitArchiveSaveOptions) | Menyimpan arsip multi-volume ke direktori tujuan yang disediakan. |

### Lihat Juga

* interface [IArchive](../iarchive/)
* namespace [Aspose.Zip](../../aspose.zip/)
* assembly [Aspose.Zip](../../)


