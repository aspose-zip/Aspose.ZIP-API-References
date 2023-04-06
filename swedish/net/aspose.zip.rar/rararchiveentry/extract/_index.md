---
title: RarArchiveEntry.Extract
second_title: Aspose.ZIP för .NET API-referens
description: RarArchiveEntry metod. Extraherar posten till filsystemet med den angivna sökvägen.
type: docs
weight: 90
url: /sv/net/aspose.zip.rar/rararchiveentry/extract/
---
## Extract(string, string) {#extract}

Extraherar posten till filsystemet med den angivna sökvägen.

```csharp
public FileInfo Extract(string path, string password = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| path | String | Sökvägen till destinationsfilen. Om filen redan finns kommer den att skrivas över. |
| password | String | Valfritt lösenord för dekryptering. |

### Returvärde

Filinformationen för den sammansatta filen.

### Undantag

| undantag | skick |
| --- | --- |
| ArgumentNullException | *path* är inget. |
| SecurityException | Den som ringer har inte den behörighet som krävs för att få åtkomst. |
| ArgumentException | De*path* är tom, innehåller bara blanksteg eller innehåller ogiltiga tecken. |
| UnauthorizedAccessException | Tillgång till fil*path* är nekad. |
| PathTooLongException | Den angivna*path*, filnamn eller båda överskrider den systemdefinierade maximala längden. Till exempel, på Windows-baserade plattformar måste sökvägar vara mindre än 248 tecken och filnamn måste vara mindre än 260 tecken. |
| NotSupportedException | Arkivera kl*path* innehåller ett kolon (:) i mitten av strängen. |
| InvalidDataException | CRC- eller MAC-verifiering misslyckades för posten. |

### Exempel

Extrahera två poster i rar-arkivet.

```csharp
using (FileStream rarFile = File.Open("archive.rar", FileMode.Open))
{
    using (RarArchive archive = new RarArchive(rarFile))
    {
        archive.Entries[0].Extract("first.bin", "pass");
        archive.Entries[1].Extract("second.bin", "pass");
    }
}
```

### Se även

* class [RarArchiveEntry](../)
* namnutrymme [Aspose.Zip.Rar](../../rararchiveentry/)
* hopsättning [Aspose.Zip](../../../)

---

## Extract(Stream, string) {#extract_1}

Extraherar posten till den tillhandahållna strömmen.

```csharp
public void Extract(Stream destination, string password = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| destination | Stream | Destinationsström. Måste vara skrivbart. |
| password | String | Valfritt lösenord för dekryptering. |

### Undantag

| undantag | skick |
| --- | --- |
| InvalidDataException | CRC- eller MAC-verifiering misslyckades för posten. |
| ArgumentException | *destination* stöder inte skrivande. |

### Exempel

Extrahera en post i rar-arkivet med lösenord.

```csharp
using (FileStream rarFile = File.Open("archive.zip", FileMode.Open))
{
    using (RarArchive archive = new RarArchive(rarFile))
    {
        archive.Entries[0].Extract(httpResponseStream, "p@s$");
    }
}
```

### Se även

* class [RarArchiveEntry](../)
* namnutrymme [Aspose.Zip.Rar](../../rararchiveentry/)
* hopsättning [Aspose.Zip](../../../)


