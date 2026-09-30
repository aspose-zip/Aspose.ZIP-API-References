---
title: "LhaArchive.LhaArchive"
second_title: "Aspose.ZIP för .NET API-referens"
description: "LhaArchive-konstruktorn. Initierar en ny instans av LhaArchive-klassen och skapar en inläggslista som kan extraheras från arkivet."
type: docs
weight: 10
url: /sv/net/aspose.zip.lha/lhaarchive/lhaarchive/
---
## LhaArchive(Stream, LhaLoadOptions) {#constructor}

Initierar en ny instans av [`LhaArchive`](../)-klassen och skapar en inläggslista som kan extraheras från arkivet.

```csharp
public LhaArchive(Stream sourceStream, LhaLoadOptions loadOptions = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceStream | Ström | Källan till arkivet. |
| loadOptions | LhaLoadOptions | Alternativ för att läsa in befintligt arkiv med. |

### Undantag

| undantag | villkor |
| --- | --- |
| ArgumentNullException | *sourceStream* är null |
| ArgumentException | *sourceStream* är ej sökbar. |
| InvalidDataException | Olämplig data hittades. |
| EndOfStreamException | Kastas när slutet av strömmen nås innan det förväntade antalet byte har lästs. |
| ObjectDisposedException | Kastas när objektet har disponerats. |

## Anmärkningar

Denna konstruktor dekomprimerar inte någon post. Se [`Extract`](../../lhaarchiveentry/extract/) metoden för dekomprimering.

### Se även

* class [LhaLoadOptions](../../lhaloadoptions/)
* class [LhaArchive](../)
* namespace [Aspose.Zip.Lha](../../lhaarchive/)
* assembly [Aspose.Zip](../../../)

---

## LhaArchive(string, LhaLoadOptions) {#constructor_1}

Initierar en ny instans av [`LhaArchive`](../)-klassen och skapar en inläggslista som kan extraheras från arkivet.

```csharp
public LhaArchive(string path, LhaLoadOptions loadOptions = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sökväg | String | Den fullständigt kvalificerade eller relativa sökvägen till arkivfilen. |
| loadOptions | LhaLoadOptions | Alternativ för att läsa in befintligt arkiv med. |

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
| InvalidDataException | Filen är korrupt. |
| EndOfStreamException | Kastas när slutet av strömmen nås innan det förväntade antalet byte har lästs. |
| ObjectDisposedException | Kastas när objektet har disponerats. |

## Anmärkningar

Denna konstruktor dekomprimerar inte någon post. Se [`Extract`](../../lhaarchiveentry/extract/) metoden för dekomprimering.

## Exempel

Följande exempel extraherar ett arkiv och dekomprimerar sedan den första posten till en `MemoryStream`.

```csharp
var extracted = new MemoryStream();
using (LhaArchive archive = new LhaArchive("sample.lzh"))
{
    archive.Entries[0].Extract(extracted);
}
```

### Se även

* class [LhaLoadOptions](../../lhaloadoptions/)
* class [LhaArchive](../)
* namespace [Aspose.Zip.Lha](../../lhaarchive/)
* assembly [Aspose.Zip](../../../)


