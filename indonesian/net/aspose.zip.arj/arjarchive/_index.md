---
title: "Kelas ArjArchive"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Kelas Aspose.Zip.Arj.ArjArchive. Kelas ini mewakili file arsip ARJ"
type: docs
weight: 250
url: /id/net/aspose.zip.arj/arjarchive/
---
## ArjArchive class

Kelas ini mewakili file arsip ARJ.

```csharp
public class ArjArchive : IArchive
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [ArjArchive](arjarchive/#constructor)(Stream, ArjLoadOptions) | Menginisialisasi instance baru dari kelas `ArjArchive` dan menyusun daftar entri yang dapat diekstrak dari arsip. |
| [ArjArchive](arjarchive/#constructor_1)(string, ArjLoadOptions) | Menginisialisasi instance baru dari kelas `ArjArchive` dan menyusun daftar entri yang dapat diekstrak dari arsip. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Commentary](../../aspose.zip.arj/arjarchive/commentary/) { get; } | Mendapatkan komentar. |
| [Entries](../../aspose.zip.arj/arjarchive/entries/) { get; } | Mendapatkan entri tipe [`ArjEntryPlain`](../arjentryplain/) yang membentuk arsip ARJ. |
| [Name](../../aspose.zip.arj/arjarchive/name/) { get; } | Mendapatkan nama asli. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Dispose](../../aspose.zip.arj/arjarchive/dispose/)() | Melakukan tugas yang ditentukan aplikasi terkait dengan membebaskan, melepaskan, atau mereset sumber daya yang tidak dikelola. |
| [ExtractToDirectory](../../aspose.zip.arj/arjarchive/extracttodirectory/)(string) | Mengekstrak semua entri ke direktori yang ditentukan. |

## Catatan

Hanya metode kompresi berikut yang didukung:

**Method**

**Explanation**

**0**

Tidak terkompresi

**1**

Kombinasi LZ77 dan pengkodean Huffman adaptif. Rasio terbaik.

**2**

Kombinasi LZ77 dan pengkodean Huffman adaptif.

**3**

Kombinasi LZ77 dan pengkodean Huffman adaptif. Kecepatan terbaik.

### Lihat Juga

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Arj](../../aspose.zip.arj/)
* assembly [Aspose.Zip](../../)


