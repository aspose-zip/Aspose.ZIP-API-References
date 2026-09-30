---
title: "Kelas IsoArchive"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Kelas Aspose.Zip.Iso.IsoArchive. Mewakili arsip ISO ISO 9660"
type: docs
weight: 570
url: /id/net/aspose.zip.iso/isoarchive/
---
## IsoArchive class

Mewakili arsip ISO (ISO 9660).

```csharp
public sealed class IsoArchive : IArchive
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [IsoArchive](isoarchive/#constructor)() | Menginisialisasi instance baru dari kelas `IsoArchive` dan membuat arsip ISO kosong untuk menambahkan file dan direktori baru. |
| [IsoArchive](isoarchive/#constructor_1)(Stream, IsoLoadOptions) | Menginisialisasi instance baru dari kelas `IsoArchive` dan menyusun daftar entri yang dapat diekstrak dari arsip. |
| [IsoArchive](isoarchive/#constructor_2)(string, IsoLoadOptions) | Menginisialisasi instance baru dari kelas `IsoArchive` dan menyusun daftar entri yang dapat diekstrak dari arsip. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Entries](../../aspose.zip.iso/isoarchive/entries/) { get; } | Mendapatkan entri tipe [`IsoEntry`](../isoentry/) yang membentuk arsip. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [CreateDirectory](../../aspose.zip.iso/isoarchive/createdirectory/)(string) | Menambahkan direktori ke gambar ISO. |
| [CreateEntry](../../aspose.zip.iso/isoarchive/createentry/#createentry)(string) | Menambahkan file ke gambar ISO. |
| [CreateEntry](../../aspose.zip.iso/isoarchive/createentry/#createentry_1)(string, Stream) | Menambahkan file ke gambar ISO. |
| [CreateEntry](../../aspose.zip.iso/isoarchive/createentry/#createentry_2)(string, string) | Menambahkan file ke gambar ISO. |
| [Dispose](../../aspose.zip.iso/isoarchive/dispose/)() | Melakukan tugas yang ditentukan aplikasi terkait dengan membebaskan, melepaskan, atau mereset sumber daya yang tidak dikelola. |
| [ExtractToDirectory](../../aspose.zip.iso/isoarchive/extracttodirectory/)(string) | Mengekstrak semua entri ke direktori yang ditentukan. |
| [Save](../../aspose.zip.iso/isoarchive/save/#save)(Stream, IsoSaveOptions) | Menyimpan gambar ISO ke aliran yang ditentukan. |
| [Save](../../aspose.zip.iso/isoarchive/save/#save_1)(string, IsoSaveOptions) | Menyimpan gambar ISO ke jalur yang ditentukan. |

### Lihat Juga

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Iso](../../aspose.zip.iso/)
* assembly [Aspose.Zip](../../)


