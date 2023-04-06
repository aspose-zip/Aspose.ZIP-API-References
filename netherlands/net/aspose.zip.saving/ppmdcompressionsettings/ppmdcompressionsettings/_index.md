---
title: PPMdCompressionSettings.PPMdCompressionSettings
second_title: Aspose.ZIP voor .NET API-referentie
description: PPMdCompressionSettings constructeur. Initialiseert een nieuw exemplaar van hetPPMdCompressionSettings klasse.
type: docs
weight: 10
url: /nl/net/aspose.zip.saving/ppmdcompressionsettings/ppmdcompressionsettings/
---
## PPMdCompressionSettings(int, int) {#constructor_1}

Initialiseert een nieuw exemplaar van het[`PPMdCompressionSettings`](../) klasse.

```csharp
public PPMdCompressionSettings(int modelOrder, int suballocatorSize)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| modelOrder | Int32 | Volgorde van het model. |
| suballocatorSize | Int32 | Geheugengrootte in MB suballocator kan verbruiken. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentOutOfRangeException | *modelOrder* ligt niet tussen 2 en 16. - of -*suballocatorSize* ligt niet tussen 1 en 256. |

### Opmerkingen

Grotere modelbestellingen resulteren vrijwel zeker in betere compressie en zeker meer geheugen en CPU-gebruik.

Het PPMd-algoritme heeft mogelijk veel geheugen nodig, vooral bij gebruik op grote bestanden en/of bij grote modelbestellingen. Als ppmd meer geheugen nodig heeft dan u eraan geeft, zal de compressie slechter zijn.

### Voorbeelden

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings(4, 10))))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### Zie ook

* class [PPMdCompressionSettings](../)
* naamruimte [Aspose.Zip.Saving](../../ppmdcompressionsettings/)
* montage [Aspose.Zip](../../../)

---

## PPMdCompressionSettings() {#constructor}

Initialiseert een nieuw exemplaar van het[`PPMdCompressionSettings`](../) klasse met standaard modelvolgorde en subtoewijzergrootte.

```csharp
public PPMdCompressionSettings()
```

### Opmerkingen

De standaardmodelvolgorde is 8 en de grootte van de subtoewijzer is 50 MB.

### Voorbeelden

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### Zie ook

* class [PPMdCompressionSettings](../)
* naamruimte [Aspose.Zip.Saving](../../ppmdcompressionsettings/)
* montage [Aspose.Zip](../../../)


