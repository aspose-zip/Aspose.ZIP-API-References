---
title: Class SelfExtractorOptions
second_title: Aspose.ZIP voor .NET API-referentie
description: Aspose.Zip.Saving.SelfExtractorOptions klas. Opties voor het maken van een zelfuitpakkend uitvoerbaar archief.
type: docs
weight: 500
url: /nl/net/aspose.zip.saving/selfextractoroptions/
---
## SelfExtractorOptions class

Opties voor het maken van een zelfuitpakkend uitvoerbaar archief.

```csharp
public class SelfExtractorOptions
```

## Constructeurs

| Naam | Beschrijving |
| --- | --- |
| [SelfExtractorOptions](selfextractoroptions/)() | De standaard constructeur. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [CloseWindowOnExtraction](../../aspose.zip.saving/selfextractoroptions/closewindowonextraction/) { get; set; } | Haalt of stelt een waarde in die aangeeft of het uitpakvenster moet worden gesloten bij het uitpakken of niet. |
| [ExtractorTitle](../../aspose.zip.saving/selfextractoroptions/extractortitle/) { get; set; } | Haalt de titel van het extractorvenster op of stelt deze in. |
| [RunAfterExtraction](../../aspose.zip.saving/selfextractoroptions/runafterextraction/) { get; set; } | Hiermee wordt een programma opgehaald of ingesteld dat moet worden uitgevoerd nadat de extractie van het archief is voltooid. |
| [TitleIcon](../../aspose.zip.saving/selfextractoroptions/titleicon/) { get; set; } | Haalt of stelt het pad naar het titelpictogram in voor de hoofdvensters van de extractortoepassing. |

### Opmerkingen

Zelfuitpakkend archief kan niet worden samengesteld met gedoseerde licentie:[`MeteredLicense`](../../aspose.zip/meteredlicense/) .

### Voorbeelden

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

### Zie ook

* naamruimte [Aspose.Zip.Saving](../../aspose.zip.saving/)
* montage [Aspose.Zip](../../)


