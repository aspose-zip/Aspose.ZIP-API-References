---
title: "LhaArchive.ExtractToDirectory"
second_title: "Aspose.ZIP för .NET API-referens"
description: "LhaArchive-metoden. Extraherar alla filer och kataloger i arkivet till den angivna katalogen."
type: docs
weight: 40
url: /sv/net/aspose.zip.lha/lhaarchive/extracttodirectory/
---
## LhaArchive.ExtractToDirectory method

Extraherar alla filer och kataloger i arkivet till den angivna katalogen.

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
| NotSupportedException | Om katalogen inte finns, innehåller sökvägen ett kolon-tecken (:) som inte är en del av en enhetsbeteckning ("C:\"). |
| ArgumentException | *destinationDirectory* är en sträng med noll längd, innehåller endast blanksteg, eller innehåller ett eller flera ogiltiga tecken. Du kan fråga efter ogiltiga tecken genom att använda metoden System.IO.Path.GetInvalidPathChars. -or- sökväg är föregången av, eller innehåller, endast ett kolon (:). |
| IOException | Katalogen som anges av path är en fil. -or- Nätverksnamnet är okänt. |
| InvalidDataException | Fel lösenord har angetts. - eller - Arkivet är korrupt. |
| OperationCanceledException | I .NET Framework 4.0 och senare: Kastas när extraktionen avbryts via den angivna avbokningstoken. |
| ObjectDisposedException | Kastas när objektet har disponerats. |

## Anmärkningar

Om katalogen inte finns kommer den att skapas.

## Exempel

```csharp
using (var archive = new LhaArchive("archive.lzh")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Se även

* class [LhaArchive](../)
* namespace [Aspose.Zip.Lha](../../lhaarchive/)
* assembly [Aspose.Zip](../../../)


