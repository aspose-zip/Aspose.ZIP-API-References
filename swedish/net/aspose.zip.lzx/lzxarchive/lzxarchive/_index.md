---
title: "LzxArchive.LzxArchive"
second_title: "Aspose.ZIP för .NET API-referens"
description: "LzxArchive-konstruktorn. Initierar en ny instans av klassen LzxArchive och skapar en postlista som kan extraheras från arkivet"
type: docs
weight: 10
url: /sv/net/aspose.zip.lzx/lzxarchive/lzxarchive/
---
## LzxArchive(Stream, LzxLoadOptions) {#constructor}

Initierar en ny instans av klassen [`LzxArchive`](../) och skapar en postlista som kan extraheras från arkivet.

```csharp
public LzxArchive(Stream extractionSource, LzxLoadOptions loadOptions = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| extractionSource | Ström | Källan till arkivet. |
| loadOptions | LzxLoadOptions | Alternativ för att läsa in befintligt arkiv med. |

### Undantag

| undantag | villkor |
| --- | --- |
| ArgumentNullException | *extractionSource* är null. |
| ArgumentException | *extractionSource* stöder inte sökning. |
| InvalidDataException | Fel signatur för arkivet. - eller - Filen är inte ett LZX-arkiv. |
| NotImplementedException | Lzx-arkivet innehåller sammanslagna poster. |
| EndOfStreamException | Strömmen *extractionSource* är för kort. |
| ObjectDisposedException | Kastas om strömmen har stängts. |
| IOException | Ett I/O‑fel inträffar. |

## Anmärkningar

Denna konstruktor dekomprimerar ingen post. Se [`Extract`](../../lzxarchiveentry/extract/) metod för dekomprimering.

### Se även

* class [LzxLoadOptions](../../lzxloadoptions/)
* class [LzxArchive](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchive/)
* assembly [Aspose.Zip](../../../)

---

## LzxArchive(string, LzxLoadOptions) {#constructor_1}

Initierar en ny instans av klassen [`LzxArchive`](../) och skapar en postlista som kan extraheras från arkivet.

```csharp
public LzxArchive(string path, LzxLoadOptions loadOptions = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sökväg | String | Den fullständigt kvalificerade eller relativa sökvägen till arkivfilen. |
| loadOptions | LzxLoadOptions | Alternativ för att läsa in befintligt arkiv med. |

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
| NotImplementedException | Lzx-arkivet innehåller sammanslagna poster. |
| EndOfStreamException | Filen är för kort. |
| ObjectDisposedException | Kastas om strömmen har stängts. |

## Anmärkningar

Denna konstruktor dekomprimerar ingen post. Se [`Extract`](../../lzxarchiveentry/extract/) metod för dekomprimering.

## Exempel

Följande exempel extraherar ett arkiv och dekomprimerar sedan den första posten till en `MemoryStream`.

```csharp
var extracted = new MemoryStream();
using (LzxArchive archive = new LzxArchive("sample.lzx"))
{
    archive.Entries[0].Extract(extracted);
}
```

### Se även

* class [LzxLoadOptions](../../lzxloadoptions/)
* class [LzxArchive](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchive/)
* assembly [Aspose.Zip](../../../)


