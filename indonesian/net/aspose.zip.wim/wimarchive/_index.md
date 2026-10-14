---
title: "Kelas WimArchive"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Aspose.Zip.Wim.WimArchive class. Kelas ini mewakili file arsip wim"
type: docs
weight: 1330
url: /id/net/aspose.zip.wim/wimarchive/
---
## WimArchive class

Kelas ini mewakili file arsip wim.

```csharp
public class WimArchive : IArchive
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [WimArchive](wimarchive/#constructor)(Stream, WimLoadOptions) | Menginisialisasi instance baru dari kelas `WimArchive` dan menyusun daftar entri yang dapat diekstrak dari arsip. |
| [WimArchive](wimarchive/#constructor_1)(string, WimLoadOptions) | Menginisialisasi instance baru dari kelas `WimArchive` dan menyusun daftar entri yang dapat diekstrak dari arsip. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [BootImageIndex](../../aspose.zip.wim/wimarchive/bootimageindex/) { get; } | Mendapatkan indeks (berbasis nol) dari gambar yang dapat di-boot. |
| [Entries](../../aspose.zip.wim/wimarchive/entries/) { get; } | Mendapatkan entri tipe [`WimEntry`](../wimentry/) yang membentuk arsip. |
| [FileFormatVersion](../../aspose.zip.wim/wimarchive/fileformatversion/) { get; } | Mendapatkan versi format file. |
| [Guid](../../aspose.zip.wim/wimarchive/guid/) { get; } | Mendapatkan GUID identifikasi untuk arsip. |
| [Images](../../aspose.zip.wim/wimarchive/images/) { get; } | Mendapatkan entri tipe [`WimImage`](../wimimage/) yang membentuk arsip. |
| [Manifest](../../aspose.zip.wim/wimarchive/manifest/) { get; } | Mendapatkan manifes tersemat yang menjelaskan file dan gambar yang terkandung. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Dispose](../../aspose.zip.wim/wimarchive/dispose/)() | Melakukan tugas yang ditentukan aplikasi terkait dengan membebaskan, melepaskan, atau mereset sumber daya yang tidak dikelola. |
| [ExtractToDirectory](../../aspose.zip.wim/wimarchive/extracttodirectory/)(string) | Mengekstrak arsip ke file berdasarkan jalur. |

### Lihat Juga

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Wim](../../aspose.zip.wim/)
* assembly [Aspose.Zip](../../)


