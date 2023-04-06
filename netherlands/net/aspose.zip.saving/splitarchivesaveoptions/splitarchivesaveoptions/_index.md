---
title: SplitArchiveSaveOptions.SplitArchiveSaveOptions
second_title: Aspose.ZIP voor .NET API-referentie
description: SplitArchiveSaveOptions constructeur. Instantiseert instellingen voor het opslaan van een ziparchief met meerdere volumes.
type: docs
weight: 10
url: /nl/net/aspose.zip.saving/splitarchivesaveoptions/splitarchivesaveoptions/
---
## SplitArchiveSaveOptions constructor

Instantiseert instellingen voor het opslaan van een zip-archief met meerdere volumes.

```csharp
public SplitArchiveSaveOptions(string fileName, uint segmentSize)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fileName | String | Naam voor delen. Mag met of zonder .zip-extensie zijn. |
| segmentSize | UInt32 | Grootte van het volume. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentOutOfRangeException | Segmentgrootte is kleiner dan 65536 bytes. |

### Opmerkingen

Sommige volumes kunnen kleiner zijn dan*segmentSize*. In de meeste gevallen zal het laatste segment minder zijn, maar in zeldzame gevallen kunnen reguliere segmenten dat ook zijn.

Namen van bestanden zijn als volgt:*fileName* .z01,*fileName* .z02, ...,*fileName* .z(n-1),*fileName*.zip.

### Zie ook

* class [SplitArchiveSaveOptions](../)
* naamruimte [Aspose.Zip.Saving](../../splitarchivesaveoptions/)
* montage [Aspose.Zip](../../../)


