---
title: "TarArchive.FromLZMA"
second_title: "Aspose.ZIP för .NET API-referens"
description: "TarArchive-metod. Extraherar angivet LZMA-arkiv och skapar ett TarArchive från den extraherade datan"
type: docs
weight: 50
url: /sv/net/aspose.zip.tar/tararchive/fromlzma/
---
## FromLZMA(Stream) {#fromlzma}

Extraherar angivet LZMA-arkiv och skapar [`TarArchive`](../) från den extraherade datan.

Viktigt: LZMA-arkivet extraheras helt inom denna metod, dess innehåll behålls internt. Var medveten om minnesanvändning.

```csharp
public static TarArchive FromLZMA(Stream source)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| källa | Ström | Källan till arkivet. |

### Returvärde

En instans av [`TarArchive`](../)

### Undantag

| undantag | villkor |
| --- | --- |
| InvalidDataException | Arkivet är skadat. |
| EndOfStreamException | Kastas när slutet av strömmen nås innan det förväntade antalet byte har lästs. |
| ObjectDisposedException | Kastas om källströmmen har frigjorts. |
| ArgumentNullException | *source* är null. |
| IOException | Ett I/O‑fel inträffar. |

## Anmärkningar

LZMA-extraktionsströmmen är inte sökbar på grund av komprimeringsalgoritmens natur. Tar-arkivet erbjuder möjlighet att extrahera godtyckliga poster, så den måste arbeta med en sökbar ström under huven.

### Se även

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## FromLZMA(string) {#fromlzma_1}

Extraherar angivet LZMA-arkiv och skapar [`TarArchive`](../) från den extraherade datan.

Viktigt: LZMA-arkivet extraheras helt inom denna metod, dess innehåll behålls internt. Var medveten om minnesanvändning.

```csharp
public static TarArchive FromLZMA(string path)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sökväg | String | Sökvägen till arkivfilen. |

### Returvärde

En instans av [`TarArchive`](../)

### Undantag

| undantag | villkor |
| --- | --- |
| ArgumentNullException | *path* är null. |
| ArgumentException | *path* är tom, innehåller bara blanksteg eller innehåller ogiltiga tecken. |
| UnauthorizedAccessException | Åtkomst till filen *path* nekas. |
| PathTooLongException | Den angivna *path*, filnamnet eller båda överskrider systemdefinierad maximal längd. Till exempel, på Windows-baserade plattformar måste sökvägar vara kortare än 248 tecken och filnamn kortare än 260 tecken. |
| NotSupportedException | Filen på *path* har ett ogiltigt format. |
| DirectoryNotFoundException | Den angivna sökvägen är ogiltig, till exempel om den ligger på en ej mappad enhet. |
| FileNotFoundException | Filen hittades inte. |
| EndOfStreamException | Kastas när slutet av strömmen nås innan det förväntade antalet byte har lästs. |
| IOException | Ett I/O‑fel inträffade när filen öppnades. |
| InvalidDataException | Arkivet är skadat. |

## Anmärkningar

LZMA-extraktionsströmmen är inte sökbar på grund av komprimeringsalgoritmens natur. Tar-arkivet erbjuder möjlighet att extrahera godtyckliga poster, så den måste arbeta med en sökbar ström under huven.

### Se även

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


