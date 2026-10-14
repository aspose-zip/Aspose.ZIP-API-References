---
title: "IsoEntry.Extract"
second_title: "Aspose.ZIP för .NET API-referens"
description: "IsoEntry metod. Extraherar posten till filsystemet med den angivna sökvägen"
type: docs
weight: 50
url: /sv/net/aspose.zip.iso/isoentry/extract/
---
## Extract(string) {#extract}

Extraherar posten till filsystemet enligt den angivna sökvägen.

```csharp
public FileInfo Extract(string path)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sökväg | String | Sökvägen till destinationsfilen. Om filen redan finns, kommer den att skrivas över. |

### Returvärde

FileInfo-instans som innehåller extraherade data.

### Undantag

| undantag | villkor |
| --- | --- |
| ArgumentNullException | *path* är null. |
| SecurityException | Anroparen har inte den erforderliga behörigheten för åtkomst. |
| ArgumentException | *path* är tom, innehåller bara blanksteg eller innehåller ogiltiga tecken. |
| UnauthorizedAccessException | Åtkomst till filen *path* nekas. |
| PathTooLongException | Den angivna *path*, filnamnet eller båda överskrider systemdefinierad maximal längd. Till exempel, på Windows-baserade plattformar måste sökvägar vara kortare än 248 tecken och filnamn kortare än 260 tecken. |
| NotSupportedException | Filen på *path* innehåller ett kolon (:) i mitten av strängen. |
| FileNotFoundException | Filen hittades inte. |
| DirectoryNotFoundException | Den angivna sökvägen är ogiltig, till exempel om den ligger på en ej mappad enhet. |
| IOException | Filen är redan öppen. |
| InvalidOperationException | Arkivhuvuden och serviceinformation lästes inte. |

### Se även

* class [IsoEntry](../)
* namespace [Aspose.Zip.Iso](../../isoentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

Extraherar posten till den angivna strömmen.

```csharp
public void Extract(Stream destination)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| mål | Ström | Destinationsström. Måste vara skrivbar. |

### Undantag

| undantag | villkor |
| --- | --- |
| NotSupportedException | Kastar ett undantag om posten inte representerar en fil. |
| ArgumentException | Den angivna strömmen stöder inte skrivning. |

### Se även

* class [IsoEntry](../)
* namespace [Aspose.Zip.Iso](../../isoentry/)
* assembly [Aspose.Zip](../../../)


