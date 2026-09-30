---
title: "Kelas Bzip2Archive"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Kelas Aspose.Zip.Bzip2.Bzip2Archive. Kelas ini mewakili file arsip bzip2. Gunakan untuk menyusun atau mengekstrak arsip bzip2"
type: docs
weight: 280
url: /id/net/aspose.zip.bzip2/bzip2archive/
---
## Bzip2Archive class

Kelas ini mewakili file arsip bzip2. Gunakan untuk membuat atau mengekstrak arsip bzip2.

```csharp
public class Bzip2Archive : IArchive, IArchiveFileEntry
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [Bzip2Archive](bzip2archive/#constructor)() | Menginisialisasi instance baru dari kelas `Bzip2Archive` yang disiapkan untuk kompresi. |
| [Bzip2Archive](bzip2archive/#constructor_1)(Stream, Bzip2LoadOptions) | Menginisialisasi instance baru dari kelas `Bzip2Archive` yang disiapkan untuk dekompresi. |
| [Bzip2Archive](bzip2archive/#constructor_2)(string, Bzip2LoadOptions) | Menginisialisasi instance baru dari kelas `Bzip2Archive` yang disiapkan untuk dekompresi. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Dispose](../../aspose.zip.bzip2/bzip2archive/dispose/)() | Melakukan tugas yang ditentukan aplikasi terkait dengan membebaskan, melepaskan, atau mereset sumber daya yang tidak dikelola. |
| [Extract](../../aspose.zip.bzip2/bzip2archive/extract/#extract_1)(Stream) | Mengekstrak arsip ke aliran yang disediakan. |
| [Extract](../../aspose.zip.bzip2/bzip2archive/extract/#extract)(string) | Mengekstrak arsip ke file berdasarkan jalur. |
| [ExtractToDirectory](../../aspose.zip.bzip2/bzip2archive/extracttodirectory/)(string) | Mengekstrak konten arsip ke direktori yang diberikan. |
| [Open](../../aspose.zip.bzip2/bzip2archive/open/)() | Membuka arsip untuk ekstraksi dan menyediakan aliran dengan konten arsip. |
| [Save](../../aspose.zip.bzip2/bzip2archive/save/#save)(Stream, Bzip2SaveOptions) | Menyimpan arsip ke aliran yang disediakan. |
| [Save](../../aspose.zip.bzip2/bzip2archive/save/#save_1)(string, Bzip2SaveOptions) | Menyimpan arsip ke file tujuan yang disediakan. |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource_2)(FileInfo) | Menetapkan konten yang akan dikompresi dalam arsip. |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource_3)(Stream) | Menetapkan konten yang akan dikompresi dalam arsip. |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource_4)(string) | Menetapkan konten yang akan dikompresi dalam arsip. |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource)(CpioArchive, CpioFormat) | Menetapkan konten yang akan dikompresi dalam arsip. |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource_1)(TarArchive, TarFormat) | Menetapkan konten yang akan dikompresi dalam arsip. |

## Catatan

bzip2 mengompresi file menggunakan algoritma kompresi teks penyortiran blok Burrows-Wheeler, dan pengkodean Huffman. Lihat selengkapnya: https://en.wikipedia.org/wiki/Bzip2

### Lihat Juga

* interface [IArchive](../../aspose.zip/iarchive/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Bzip2](../../aspose.zip.bzip2/)
* assembly [Aspose.Zip](../../)


