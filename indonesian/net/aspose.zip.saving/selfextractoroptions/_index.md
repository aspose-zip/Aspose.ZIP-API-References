---
title: "Kelas SelfExtractorOptions"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Kelas Aspose.Zip.Saving.SelfExtractorOptions. Opsi untuk pembuatan arsip eksekutabel yang dapat mengekstrak sendiri"
type: docs
weight: 1000
url: /id/net/aspose.zip.saving/selfextractoroptions/
---
## SelfExtractorOptions class

Opsi untuk pembuatan arsip eksekutabel yang dapat mengekstrak sendiri.

```csharp
public class SelfExtractorOptions
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [SelfExtractorOptions](selfextractoroptions/)() | Konstruktor default. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [CloseWindowOnExtraction](../../aspose.zip.saving/selfextractoroptions/closewindowonextraction/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah jendela ekstraktor harus ditutup setelah ekstraksi atau tidak. |
| [ExtractorTitle](../../aspose.zip.saving/selfextractoroptions/extractortitle/) { get; set; } | Mendapatkan atau mengatur judul jendela ekstraktor. |
| [RunAfterExtraction](../../aspose.zip.saving/selfextractoroptions/runafterextraction/) { get; set; } | Mendapatkan atau mengatur program yang akan dijalankan setelah ekstraksi arsip selesai. |
| [TitleIcon](../../aspose.zip.saving/selfextractoroptions/titleicon/) { get; set; } | Mendapatkan atau mengatur jalur ke ikon judul untuk jendela utama aplikasi ekstraktor. |

## Contoh

```csharp
using (FileStream zipFile = File.Open("archive.exe", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry.bin", "data.bin");
        var sfxOptions = new SelfExtractorOptions() { ExtractorTitle = "Extractor", CloseWindowOnExtraction = true, TitleIcon = "C:\pictogram.ico" };
        archive.Save(zipFile, new ArchiveSaveOptions() { SelfExtractorOptions = sfxOptions });
    }
}
```

### Lihat Juga

* namespace [Aspose.Zip.Saving](../../aspose.zip.saving/)
* assembly [Aspose.Zip](../../)


