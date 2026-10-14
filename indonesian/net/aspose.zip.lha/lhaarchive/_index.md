---
title: "Kelas LhaArchive"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Kelas Aspose.Zip.Lha.LhaArchive. Kelas ini mewakili file arsip LHA .lzh"
type: docs
weight: 630
url: /id/net/aspose.zip.lha/lhaarchive/
---
## LhaArchive class

Kelas ini mewakili file arsip LHA (.lzh).

```csharp
public class LhaArchive : IArchive
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [LhaArchive](lhaarchive/#constructor)(Stream, LhaLoadOptions) | Menginisialisasi instance baru dari kelas `LhaArchive` dan menyusun daftar entri yang dapat diekstrak dari arsip. |
| [LhaArchive](lhaarchive/#constructor_1)(string, LhaLoadOptions) | Menginisialisasi instance baru dari kelas `LhaArchive` dan menyusun daftar entri yang dapat diekstrak dari arsip. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Entries](../../aspose.zip.lha/lhaarchive/entries/) { get; } | Mendapatkan entri file tipe [`LhaArchiveEntry`](../lhaarchiveentry/) yang membentuk arsip. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Dispose](../../aspose.zip.lha/lhaarchive/dispose/)() |  |
| [ExtractToDirectory](../../aspose.zip.lha/lhaarchive/extracttodirectory/)(string) | Mengekstrak semua file dan direktori dalam arsip ke direktori yang diberikan. |

## Catatan

Hanya metode kompresi berikut yang didukung:

**Method**

**Explanation**

**lh0**

Tidak terkompresi

**lh4**

Kamus geser 8 KiB dan Huffman statis

**lh5**

Kamus geser 16 KiB dan Huffman statis

**lh6**

Kamus geser 64 KiB dan Huffman statis

**lh7**

Kamus geser 128 KiB dan Huffman statis

**lhx**

Kamus geser 1 Mib dan Huffman statis

**lhd**

Direktori

### Lihat Juga

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Lha](../../aspose.zip.lha/)
* assembly [Aspose.Zip](../../)


