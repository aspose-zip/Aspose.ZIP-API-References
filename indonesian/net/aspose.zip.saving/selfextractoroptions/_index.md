---
title: Class SelfExtractorOptions
second_title: Aspose.ZIP untuk Referensi .NET API
description: Aspose.Zip.Saving.SelfExtractorOptions kelas. Opsi untuk membuat arsip yang dapat dieksekusi yang dapat diekstrak sendiri.
type: docs
weight: 500
url: /id/net/aspose.zip.saving/selfextractoroptions/
---
## SelfExtractorOptions class

Opsi untuk membuat arsip yang dapat dieksekusi yang dapat diekstrak sendiri.

```csharp
public class SelfExtractorOptions
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [SelfExtractorOptions](selfextractoroptions/)() | Konstruktor default. |

## Properti

| Nama | Keterangan |
| --- | --- |
| [CloseWindowOnExtraction](../../aspose.zip.saving/selfextractoroptions/closewindowonextraction/) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah jendela ekstraktor harus ditutup saat ekstraksi atau tidak. |
| [ExtractorTitle](../../aspose.zip.saving/selfextractoroptions/extractortitle/) { get; set; } | Mendapat atau menyetel judul jendela ekstraktor. |
| [RunAfterExtraction](../../aspose.zip.saving/selfextractoroptions/runafterextraction/) { get; set; } | Mendapat atau mengatur program yang akan dijalankan setelah ekstraksi arsip selesai. |
| [TitleIcon](../../aspose.zip.saving/selfextractoroptions/titleicon/) { get; set; } | Mendapat atau menyetel jalur ke ikon judul untuk jendela utama aplikasi ekstraktor. |

### Perkataan

Arsip yang mengekstraksi sendiri tidak dapat dibuat dengan lisensi terukur:[`MeteredLicense`](../../aspose.zip/meteredlicense/) .

### Contoh

```csharp
using (FileStream zipFile = File.Open("archive.exe", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry.bin", "data.bin");
        var sfxOptions = new SelfExtractorOptions() { ExtractorTitle = "Extractor", CloseWindowOnExtraction = true, TitleIcon = "C:\pictorgam.ico" };
        archive.Save(zipFile, new ArchiveSaveOptions() { SelfExtractorOptions = sfxOptions });
    }
}
```

### Lihat juga

* ruang nama [Aspose.Zip.Saving](../../aspose.zip.saving/)
* perakitan [Aspose.Zip](../../)


