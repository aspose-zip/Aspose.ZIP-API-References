---
title: "TarArchive.FromLZ4"
second_title: "Aspose.ZIP för .NET API-referens"
description: "TarArchive-metod. Extraherar angivet LZ4-arkiv och bygger ett TarArchive från den extraherade datan"
type: docs
weight: 30
url: /sv/net/aspose.zip.tar/tararchive/fromlz4/
---
## FromLZ4(string) {#fromlz4_1}

Extraherar angivet LZ4-arkiv och bygger [`TarArchive`](../) från den extraherade datan.

Viktigt: LZ4-arkivet extraheras helt inom denna metod, dess innehåll behålls internt. Se upp för minnesanvändning.

```csharp
public static TarArchive FromLZ4(string path)
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
| SecurityException | Anroparen har inte den nödvändiga behörigheten för åtkomst |
| ArgumentException | *path* är tom, innehåller bara blanksteg eller innehåller ogiltiga tecken. |
| UnauthorizedAccessException | Åtkomst till filen *path* nekas. |
| PathTooLongException | Den angivna *path*, filnamnet eller båda överskrider systemdefinierad maximal längd. Till exempel, på Windows-baserade plattformar måste sökvägar vara kortare än 248 tecken och filnamn kortare än 260 tecken. |
| NotSupportedException | Filen på *path* har ett ogiltigt format. |
| DirectoryNotFoundException | Den angivna sökvägen är ogiltig, till exempel om den ligger på en ej mappad enhet. |
| FileNotFoundException | Filen hittades inte. |
| EndOfStreamException | Filen är för kort. |
| InvalidDataException | Filen har fel signatur. |
| IOException | Ett I/O‑fel inträffade när filen öppnades. |
| InvalidOperationException | Arkivet är förberett för sammansättning. |

## Anmärkningar

LZ4-extraheringsström är inte sökbar på grund av komprimeringsalgoritmens natur. Tar-arkivet erbjuder möjlighet att extrahera godtyckliga poster, så det måste arbeta med en sökbar ström under huven.

### Se även

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## FromLZ4(Stream) {#fromlz4}

Extraherar angivet LZ4-arkiv och bygger [`TarArchive`](../) från den extraherade datan.

Viktigt: LZ4-arkivet extraheras helt inom denna metod, dess innehåll behålls internt. Se upp för minnesanvändning.

```csharp
public static TarArchive FromLZ4(Stream source)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| källa | Ström | Källan till arkivet. |

### Returvärde

En instans av [`TarArchive`](../)

### Undantag

| undantag | villkor |
| --- | --- |
| ArgumentException | Kan inte läsa från *source* |
| ArgumentNullException | *source* är null. |
| EndOfStreamException | *source* är för kort. |
| InvalidDataException | Den *source* har fel signatur. |
| ObjectDisposedException | Kastas om källströmmen har frigjorts. |

## Anmärkningar

LZ4-extraheringsström är inte sökbar på grund av komprimeringsalgoritmens natur. Tar-arkivet erbjuder möjlighet att extrahera godtyckliga poster, så det måste arbeta med en sökbar ström under huven.

### Se även

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


