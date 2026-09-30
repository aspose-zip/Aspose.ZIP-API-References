---
title: "IArchive.ExtractToDirectory"
second_title: "Aspose.ZIP för .NET API-referens"
description: "IArchive-metod. Extraherar alla filer i arkivet till den angivna katalogen."
type: docs
weight: 30
url: /sv/net/aspose.zip/iarchive/extracttodirectory/
---
## IArchive.ExtractToDirectory method

Extraherar alla filer i arkivet till den angivna katalogen.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| destinationDirectory | String | Sökvägen till katalogen där de extraherade filerna ska placeras. |

### Undantag

| undantag | villkor |
| --- | --- |
| ArgumentNullException | *destinationDirectory* är null. |
| PathTooLongException | Den angivna sökvägen, filnamnet eller båda överskrider systemets maximala längd. Till exempel, på Windows‑baserade plattformar måste sökvägar vara kortare än 248 tecken och filnamn kortare än 260 tecken. |
| SecurityException | Anroparen har inte den nödvändiga behörigheten för att komma åt den befintliga katalogen. |
| NotSupportedException | Om katalogen inte finns, innehåller en sökväg ett kolon (:) som inte är en del av en enhetsetikett ("C:\"). |
| ArgumentException | *destinationDirectory* är en sträng med noll längd, innehåller endast blanksteg, eller innehåller ett eller flera ogiltiga tecken. Du kan fråga efter ogiltiga tecken genom att använda metoden System.IO.Path.GetInvalidPathChars. -or- sökväg är föregången av, eller innehåller, endast ett kolon (:). |
| IOException | Katalogen som anges av path är en fil. -or- Nätverksnamnet är okänt. |

## Anmärkningar

Om katalogen inte finns kommer den att skapas.

### Se även

* interface [IArchive](../)
* namespace [Aspose.Zip](../../iarchive/)
* assembly [Aspose.Zip](../../../)


