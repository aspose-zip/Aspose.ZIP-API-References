---
title: XarArchive.ExtractToDirectory
second_title: Aspose.ZIP för .NET API-referens
description: XarArchive metod. Extraherar alla filer i arkivet till den angivna katalogen.
type: docs
weight: 40
url: /sv/net/aspose.zip.xar/xararchive/extracttodirectory/
---
## XarArchive.ExtractToDirectory method

Extraherar alla filer i arkivet till den angivna katalogen.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| destinationDirectory | String | Sökvägen till katalogen att placera de extraherade filerna i. |

### Undantag

| undantag | skick |
| --- | --- |
| ArgumentNullException | sökvägen är null |
| PathTooLongException | Den angivna sökvägen, filnamnet eller båda överskrider den systemdefinierade maximala längden. Till exempel, på Windows-baserade plattformar måste sökvägar vara mindre än 248 tecken och filnamn måste vara mindre än 260 tecken. |
| SecurityException | Den som ringer har inte den behörighet som krävs för att komma åt befintlig katalog. |
| NotSupportedException | Om katalogen inte finns innehåller sökvägen ett kolontecken (:) som inte är en del av en enhetsetikett ("C:\"). |
| ArgumentException | sökvägen är en sträng av noll längd, innehåller endast blanksteg eller innehåller ett eller flera ogiltiga tecken. Du kan fråga efter ogiltiga tecken genom att använda metoden System.IO.Path.GetInvalidPathChars. -eller- sökväg har prefixet med eller innehåller endast ett kolontecken (:). |
| IOException | Katalogen som anges av sökvägen är en fil. -eller- Nätverkets namn är inte känt. |

### Anmärkningar

Om katalogen inte finns skapas den.

### Exempel

```csharp
using (var archive = new XarArchive("archive.xar")) 
{
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Se även

* class [XarArchive](../)
* namnutrymme [Aspose.Zip.Xar](../../xararchive/)
* hopsättning [Aspose.Zip](../../../)


