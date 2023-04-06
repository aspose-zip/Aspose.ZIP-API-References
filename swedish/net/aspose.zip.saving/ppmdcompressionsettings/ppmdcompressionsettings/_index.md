---
title: PPMdCompressionSettings.PPMdCompressionSettings
second_title: Aspose.ZIP för .NET API-referens
description: PPMdCompressionSettings byggare. Initierar en ny instans avPPMdCompressionSettings class.
type: docs
weight: 10
url: /sv/net/aspose.zip.saving/ppmdcompressionsettings/ppmdcompressionsettings/
---
## PPMdCompressionSettings(int, int) {#constructor_1}

Initierar en ny instans av[`PPMdCompressionSettings`](../) class.

```csharp
public PPMdCompressionSettings(int modelOrder, int suballocatorSize)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| modelOrder | Int32 | Beställning av modellen. |
| suballocatorSize | Int32 | Minnesstorlek i MB suballocator kan förbruka. |

### Undantag

| undantag | skick |
| --- | --- |
| ArgumentOutOfRangeException | *modelOrder* är inte mellan 2 och 16. - eller -*suballocatorSize* är inte mellan 1 och 256. |

### Anmärkningar

Större modellbeställningar resulterar nästan säkert i bättre komprimering och säkert mer minne och CPU-användning.

PPMd-algoritmen kan behöva mycket minne, speciellt när den används på stora filer och/eller används med stor modellbeställning. Om ppmd behöver mer minne än du ger den, blir komprimeringen sämre.

### Exempel

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings(4, 10))))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### Se även

* class [PPMdCompressionSettings](../)
* namnutrymme [Aspose.Zip.Saving](../../ppmdcompressionsettings/)
* hopsättning [Aspose.Zip](../../../)

---

## PPMdCompressionSettings() {#constructor}

Initierar en ny instans av[`PPMdCompressionSettings`](../) klass med standardmodellordning och underfördelarstorlek.

```csharp
public PPMdCompressionSettings()
```

### Anmärkningar

Standardmodellbeställningen är 8 och underfördelarens storlek är 50 MB.

### Exempel

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### Se även

* class [PPMdCompressionSettings](../)
* namnutrymme [Aspose.Zip.Saving](../../ppmdcompressionsettings/)
* hopsättning [Aspose.Zip](../../../)


