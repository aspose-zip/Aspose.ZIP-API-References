---
title: SevenZipPPMdCompressionSettings.SevenZipPPMdCompressionSettings
second_title: Aspose.ZIP för .NET API-referens
description: SevenZipPPMdCompressionSettings byggare. Instantierar inställningar för PPMdkomprimeringsmetod inom 7zarkiv.
type: docs
weight: 10
url: /sv/net/aspose.zip.saving/sevenzipppmdcompressionsettings/sevenzipppmdcompressionsettings/
---
## SevenZipPPMdCompressionSettings(byte, int) {#constructor_1}

Instantierar inställningar för PPMd-komprimeringsmetod inom 7z-arkiv.

```csharp
public SevenZipPPMdCompressionSettings(byte maxOrder, int suballocatorSize)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| maxOrder | Byte | Maximal beställning. |
| suballocatorSize | Int32 | Minnesstorlek i MB suballocator kan förbruka. |

### Undantag

| undantag | skick |
| --- | --- |
| ArgumentOutOfRangeException | *maxOrder* är inte mellan 2 och 32, eller*suballocatorSize* är inte mellan 1 och 1024. |

### Anmärkningar

Större modellbeställningar resulterar nästan säkert i bättre komprimering och säkert mer minne och CPU-användning.

PPMd-algoritmen kan behöva mycket minne, speciellt när den används på stora filer och/eller används med stor modellbeställning. Om ppmd behöver mer minne än du ger den, blir komprimeringen sämre.

### Exempel

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings(4, 32))))
{
    archive.CreateEntry("data.bin", "data.bin");                        
    archive.Save(sevenZipFile);
 }
```

### Se även

* class [SevenZipPPMdCompressionSettings](../)
* namnutrymme [Aspose.Zip.Saving](../../sevenzipppmdcompressionsettings/)
* hopsättning [Aspose.Zip](../../../)

---

## SevenZipPPMdCompressionSettings() {#constructor}

Instantierar inställningar för PPMd-komprimeringsmetod inom 7z-arkiv med standardmodellordning och underallokatorstorlek.

```csharp
public SevenZipPPMdCompressionSettings()
```

### Anmärkningar

Standardmodellbeställningen är 6 och underfördelarens storlek är 16 MB.

### Exempel

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                        
    archive.Save(sevenZipFile);
 }
```

### Se även

* class [SevenZipPPMdCompressionSettings](../)
* namnutrymme [Aspose.Zip.Saving](../../sevenzipppmdcompressionsettings/)
* hopsättning [Aspose.Zip](../../../)


