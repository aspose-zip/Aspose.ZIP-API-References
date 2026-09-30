---
title: "EggArchive.EggArchive"
second_title: "Aspose.ZIP för .NET API-referens"
description: "EggArchive-konstruktor. Initierar en ny instans av EggArchive-klassen från en ström"
type: docs
weight: 10
url: /sv/net/aspose.zip.egg/eggarchive/eggarchive/
---
## EggArchive(Stream, EggArchiveLoadOptions) {#constructor}

Initierar en ny instans av [`EggArchive`](../) klassen från en ström.

```csharp
public EggArchive(Stream stream, EggArchiveLoadOptions loadOptions = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | Ström | EGG-arkivströmmen. Strömmen måste stödja läsning och sökning. |
| loadOptions | EggArchiveLoadOptions | Alternativ för att ladda arkivet med. |

### Undantag

| undantag | villkor |
| --- | --- |
| ArgumentNullException | *stream* är null. |
| ArgumentException | *stream* är inte läsbar och sökbar. |

### Se även

* class [EggArchiveLoadOptions](../../eggarchiveloadoptions/)
* class [EggArchive](../)
* namespace [Aspose.Zip.Egg](../../eggarchive/)
* assembly [Aspose.Zip](../../../)

---

## EggArchive(string, EggArchiveLoadOptions) {#constructor_1}

Initierar en ny instans av klassen [`EggArchive`](../) från en filsökväg.

```csharp
public EggArchive(string path, EggArchiveLoadOptions loadOptions = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sökväg | String | Sökväg till EGG-arkivfilen. |
| loadOptions | EggArchiveLoadOptions | Alternativ för att ladda arkivet med. |

### Undantag

| undantag | villkor |
| --- | --- |
| ArgumentNullException | *path* är null. |
| FileNotFoundException | Filen finns inte. |
| SecurityException | Anroparen har inte den erforderliga behörigheten för åtkomst. |
| ArgumentException | *path* är tom, innehåller bara blanksteg eller innehåller ogiltiga tecken. |
| UnauthorizedAccessException | Åtkomst till filen *path* nekas. |
| PathTooLongException | Den angivna *path*, filnamnet eller båda överskrider systemdefinierad maximal längd. Till exempel, på Windows-baserade plattformar måste sökvägar vara kortare än 248 tecken och filnamn kortare än 260 tecken. |
| NotSupportedException | Filen på *path* innehåller ett kolon (:) i mitten av strängen. |
| FileNotFoundException | Filen hittades inte. |
| DirectoryNotFoundException | Den angivna sökvägen är ogiltig, till exempel om den ligger på en ej mappad enhet. |
| IOException | Filen är redan öppen. |

### Se även

* class [EggArchiveLoadOptions](../../eggarchiveloadoptions/)
* class [EggArchive](../)
* namespace [Aspose.Zip.Egg](../../eggarchive/)
* assembly [Aspose.Zip](../../../)


