---
title: SplitSevenZipArchiveSaveOptions.SplitSevenZipArchiveSaveOptions
second_title: Aspose.ZIP voor .NET API-referentie
description: SplitSevenZipArchiveSaveOptions constructeur. Instantiseert instellingen voor het opslaan van een 7zarchief met meerdere volumes.
type: docs
weight: 10
url: /nl/net/aspose.zip.saving/splitsevenziparchivesaveoptions/splitsevenziparchivesaveoptions/
---
## SplitSevenZipArchiveSaveOptions constructor

Instantiseert instellingen voor het opslaan van een 7z-archief met meerdere volumes.

```csharp
public SplitSevenZipArchiveSaveOptions(string fileName, uint segmentSize)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fileName | String | Naam voor delen. Mag met of zonder .7z-extensie zijn. |
| segmentSize | UInt32 | Grootte van het volume. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentOutOfRangeException | *segmentSize* bedraagt minder dan 100. |

### Opmerkingen

Sommige volumes kunnen kleiner zijn dan*segmentSize*. In de meeste gevallen zal het laatste segment minder zijn, maar in zeldzame gevallen kunnen reguliere segmenten dat ook zijn.

Namen van bestanden zijn als volgt:*fileName* .7z.001,*fileName* .7z.002, ...,*fileName*.7z.(n).

### Zie ook

* class [SplitSevenZipArchiveSaveOptions](../)
* naamruimte [Aspose.Zip.Saving](../../splitsevenziparchivesaveoptions/)
* montage [Aspose.Zip](../../../)


