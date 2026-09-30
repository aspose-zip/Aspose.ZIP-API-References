---
title: "GzipArchive.ExtractToDirectory"
second_title: "Aspose.ZIP för .NET API-referens"
description: "GzipArchive‑metod. Extraherar arkivets innehåll till den angivna katalogen."
type: docs
weight: 60
url: /sv/net/aspose.zip.gzip/gziparchive/extracttodirectory/
---
## GzipArchive.ExtractToDirectory method

Extraherar arkivinnehållet till den angivna katalogen.

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
| NotSupportedException | Om katalogen inte finns, innehåller sökvägen ett kolon (:) som inte är en del av en enhetsbeteckning (\"C:\\\"). |
| ArgumentException | *destinationDirectory* är en sträng med noll längd, innehåller endast blanksteg, eller innehåller ett eller flera ogiltiga tecken. Du kan fråga efter ogiltiga tecken genom att använda metoden System.IO.Path.GetInvalidPathChars. -or- sökväg är föregången av, eller innehåller, endast ett kolon (:). |
| IOException | Katalogen som anges av path är en fil. -or- Nätverksnamnet är okänt. |
| OperationCanceledException | I .NET Framework 4.0 och senare: Kastas när extraktionen avbryts via den angivna avbokningstoken. |
| ObjectDisposedException | Arkivet har frigjorts och kan inte användas. |

## Anmärkningar

Om katalogen inte finns kommer den att skapas.

### Se även

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)


