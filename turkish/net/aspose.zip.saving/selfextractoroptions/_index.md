---
title: Class SelfExtractorOptions
second_title: Aspose.ZIP for .NET API Referansı
description: Aspose.Zip.Saving.SelfExtractorOptions sınıf. Kendi kendine açılan yürütülebilir arşiv oluşturma seçenekleri.
type: docs
weight: 500
url: /tr/net/aspose.zip.saving/selfextractoroptions/
---
## SelfExtractorOptions class

Kendi kendine açılan yürütülebilir arşiv oluşturma seçenekleri.

```csharp
public class SelfExtractorOptions
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [SelfExtractorOptions](selfextractoroptions/)() | Default_Constructor |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [CloseWindowOnExtraction](../../aspose.zip.saving/selfextractoroptions/closewindowonextraction/) { get; set; } | Ayıklama sırasında çıkarıcı penceresinin kapatılması gerekip gerekmediğini gösteren bir değer alır veya ayarlar. |
| [ExtractorTitle](../../aspose.zip.saving/selfextractoroptions/extractortitle/) { get; set; } | Çıkarıcı penceresinin başlığını alır veya ayarlar. |
| [RunAfterExtraction](../../aspose.zip.saving/selfextractoroptions/runafterextraction/) { get; set; } | Arşiv çıkarma işlemi tamamlandıktan sonra yürütülecek bir program alır veya ayarlar. |
| [TitleIcon](../../aspose.zip.saving/selfextractoroptions/titleicon/) { get; set; } | Çıkarıcı uygulamasının ana pencereleri için başlık simgesine giden yolu alır veya ayarlar. |

### Notlar

Kendiliğinden açılan arşiv ölçülü lisansla oluşturulamaz:[`MeteredLicense`](../../aspose.zip/meteredlicense/) .

### Örnekler

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

### Ayrıca bakınız

* ad alanı [Aspose.Zip.Saving](../../aspose.zip.saving/)
* toplantı [Aspose.Zip](../../)


