---
title: SevenZipLZMA2CompressionSettings.SevenZipLZMA2CompressionSettings
second_title: Aspose.ZIP voor .NET API-referentie
description: SevenZipLZMA2CompressionSettings constructeur. Instantiseert instellingen voor LZMA2compressiemethode binnen 7zarchief.
type: docs
weight: 10
url: /nl/net/aspose.zip.saving/sevenziplzma2compressionsettings/sevenziplzma2compressionsettings/
---
## SevenZipLZMA2CompressionSettings(int) {#constructor}

Instantiseert instellingen voor LZMA2-compressiemethode binnen 7z-archief.

```csharp
public SevenZipLZMA2CompressionSettings(int dictionarySize = 16777216)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| dictionarySize | Int32 | Grootte van geschiedenisbuffer, moet tussen 4096 en 1073741824 liggen. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentOutOfRangeException | *dictionarySize* is te groot of te klein. |

### Opmerkingen

Hoe groter het woordenboek, hoe beter de compressieverhouding gewoonlijk is, maar woordenboeken die groter zijn dan de niet-gecomprimeerde gegevens zijn verspilling van RAM.

### Zie ook

* class [SevenZipLZMA2CompressionSettings](../)
* naamruimte [Aspose.Zip.Saving](../../sevenziplzma2compressionsettings/)
* montage [Aspose.Zip](../../../)

---

## SevenZipLZMA2CompressionSettings(int, int) {#constructor_1}

Instantiseert instellingen voor LZMA2-compressiemethode binnen 7z-archief.

```csharp
public SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes = 32)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| dictionarySize | Int32 | Grootte van geschiedenisbuffer, moet tussen 4096 en 1073741824 liggen. |
| fastBytes | Int32 | Regelt het aantal snelle bytes dat wordt gebruikt door de LZMA2-compressoren. Een groter aantal snelle bytes kan een betere compressieverhouding opleveren ten koste van de compressiesnelheid. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentOutOfRangeException | *dictionarySize* is te groot of te klein, of*fastBytes* is te groot of te klein. |

### Opmerkingen

Hoe groter het woordenboek, hoe beter de compressieverhouding gewoonlijk is, maar woordenboeken die groter zijn dan de niet-gecomprimeerde gegevens zijn verspilling van RAM.

### Zie ook

* class [SevenZipLZMA2CompressionSettings](../)
* naamruimte [Aspose.Zip.Saving](../../sevenziplzma2compressionsettings/)
* montage [Aspose.Zip](../../../)


