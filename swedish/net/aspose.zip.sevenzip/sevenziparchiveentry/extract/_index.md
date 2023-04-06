---
title: SevenZipArchiveEntry.Extract
second_title: Aspose.ZIP för .NET API-referens
description: SevenZipArchiveEntry metod. Extraherar posten till filsystemet med den angivna sökvägen.
type: docs
weight: 80
url: /sv/net/aspose.zip.sevenzip/sevenziparchiveentry/extract/
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

### Exempel

```csharp
using (var archive = new SevenZipArchive("archive.7z"))
{
    archive.Entries[0].Extract("data.bin");
}
```

### Se även

* class [SevenZipArchiveEntry](../)
* namnutrymme [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
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
| ArgumentException | *destination* stöder inte skrivande. |
| InvalidOperationException | Arkivet öppnas inte för utvinning. - eller - Denna post är en katalog. |
| InvalidDataException | Fel data i posten. |

### Exempel

Extrahera en post i zip-arkivet med lösenord.

```csharp
using (var archive = new SevenZipArchive("archive.7z"))
{
    archive.Entries[0].Extract(httpResponseStream);
}
```

### Se även

* class [SevenZipArchiveEntry](../)
* namnutrymme [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* hopsättning [Aspose.Zip](../../../)


