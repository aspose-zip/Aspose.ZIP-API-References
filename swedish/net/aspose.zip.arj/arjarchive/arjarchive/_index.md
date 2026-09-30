---
title: "ArjArchive.ArjArchive"
second_title: "Aspose.ZIP för .NET API-referens"
description: "ArjArchive‑konstruktor. Initierar en ny instans av klassen ArjArchive och skapar en postlista som kan extraheras från arkivet."
type: docs
weight: 10
url: /sv/net/aspose.zip.arj/arjarchive/arjarchive/
---
## ArjArchive(Stream, ArjLoadOptions) {#constructor}

Initierar en ny instans av klassen [`ArjArchive`](../) och skapar en postlista som kan extraheras från arkivet.

```csharp
public ArjArchive(Stream extractionSource, ArjLoadOptions loadOptions = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| extractionSource | Ström | Källan till arkivet. |
| loadOptions | ArjLoadOptions | Alternativ för att läsa in befintligt arkiv med. |

### Undantag

| undantag | villkor |
| --- | --- |
| ArgumentNullException | *extractionSource* är null. |
| ArgumentException | &gt;*extractionSource* stöder inte sökning. |
| InvalidDataException | Fel signatur för arkivet. - eller - Filen är inte ett ARJ‑arkiv. |
| EndOfStreamException | Kastas när slutet på strömmen nås innan alla header‑byte eller namn‑byte har lästs. |
| NotSupportedException | Arkivet är förvrängt. |

## Anmärkningar

Den här konstruktorn dekomprimerar inte någon post. Se [`Extract`](../../arjentryplain/extract/) metod för dekomprimering.

### Se även

* class [ArjLoadOptions](../../arjloadoptions/)
* class [ArjArchive](../)
* namespace [Aspose.Zip.Arj](../../arjarchive/)
* assembly [Aspose.Zip](../../../)

---

## ArjArchive(string, ArjLoadOptions) {#constructor_1}

Initierar en ny instans av klassen [`ArjArchive`](../) och skapar en postlista som kan extraheras från arkivet.

```csharp
public ArjArchive(string path, ArjLoadOptions loadOptions = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sökväg | String | Sökvägen till arkivfilen. |
| loadOptions | ArjLoadOptions | Alternativ för att läsa in befintligt arkiv med. |

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
| EndOfStreamException | Kastas när slutet på strömmen nås innan alla header‑byte eller namn‑byte har lästs. |
| InvalidDataException | ARJ‑magiska talet är ogiltigt eller header‑storleken är utanför intervallet. |

## Anmärkningar

Den här konstruktorn packar inte upp någon post. Se [`Extract`](../../arjentryplain/extract/) metod för dekomprimering.

## Exempel

Följande exempel visar hur man extraherar alla poster till en katalog.

```csharp
using (var archive = new ArjArchive("archive.arj")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Se även

* class [ArjLoadOptions](../../arjloadoptions/)
* class [ArjArchive](../)
* namespace [Aspose.Zip.Arj](../../arjarchive/)
* assembly [Aspose.Zip](../../../)


