---
title: SevenZipPPMdCompressionSettings.SevenZipPPMdCompressionSettings
second_title: Aspose.ZIP voor .NET API-referentie
description: SevenZipPPMdCompressionSettings constructeur. Instantiseert instellingen voor PPMdcompressiemethode binnen 7zarchief.
type: docs
weight: 10
url: /nl/net/aspose.zip.saving/sevenzipppmdcompressionsettings/sevenzipppmdcompressionsettings/
---
## SevenZipPPMdCompressionSettings(byte, int) {#constructor_1}

Instantiseert instellingen voor PPMd-compressiemethode binnen 7z-archief.

```csharp
public SevenZipPPMdCompressionSettings(byte maxOrder, int suballocatorSize)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| maxOrder | Byte | Maximale bestelling. |
| suballocatorSize | Int32 | Geheugengrootte in MB suballocator kan verbruiken. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentOutOfRangeException | *maxOrder* niet tussen 2 en 32 ligt, of*suballocatorSize* ligt niet tussen 1 en 1024. |

### Opmerkingen

Grotere modelbestellingen resulteren vrijwel zeker in betere compressie en zeker meer geheugen en CPU-gebruik.

Het PPMd-algoritme heeft mogelijk veel geheugen nodig, vooral bij gebruik op grote bestanden en/of bij grote modelbestellingen. Als ppmd meer geheugen nodig heeft dan u eraan geeft, zal de compressie slechter zijn.

### Voorbeelden

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings(4, 32))))
{
    archive.CreateEntry("data.bin", "data.bin");                        
    archive.Save(sevenZipFile);
 }
```

### Zie ook

* class [SevenZipPPMdCompressionSettings](../)
* naamruimte [Aspose.Zip.Saving](../../sevenzipppmdcompressionsettings/)
* montage [Aspose.Zip](../../../)

---

## SevenZipPPMdCompressionSettings() {#constructor}

Instantiseert instellingen voor PPMd-compressiemethode binnen 7z-archief met standaard modelvolgorde en subtoewijzergrootte.

```csharp
public SevenZipPPMdCompressionSettings()
```

### Opmerkingen

De standaardmodelvolgorde is 6 en de grootte van de subtoewijzer is 16 MB.

### Voorbeelden

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                        
    archive.Save(sevenZipFile);
 }
```

### Zie ook

* class [SevenZipPPMdCompressionSettings](../)
* naamruimte [Aspose.Zip.Saving](../../sevenzipppmdcompressionsettings/)
* montage [Aspose.Zip](../../../)


