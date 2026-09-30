---
title: "TarArchive.FromZstandard"
second_title: "Aspose.ZIP för .NET API-referens"
description: "TarArchive-metod. Extraherar angivet Zstandard-arkiv och skapar ett TarArchive från den extraherade datan"
type: docs
weight: 80
url: /sv/net/aspose.zip.tar/tararchive/fromzstandard/
---
## FromZstandard(Stream) {#fromzstandard}

Extraherar angivet Zstandard-arkiv och skapar [`TarArchive`](../) från den extraherade datan.

Viktigt: Zstandard-arkivet extraheras helt inom denna metod, dess innehåll behålls internt. Var medveten om minnesanvändning.

```csharp
public static TarArchive FromZstandard(Stream source)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| källa | Ström | Källan till arkivet. |

### Returvärde

En instans av [`TarArchive`](../)

### Undantag

| undantag | villkor |
| --- | --- |
| IOException | Zstandard-strömmen är skadad eller kan inte läsas. |
| InvalidDataException | Data är skadad. |
| EndOfStreamException | Kastas när slutet av strömmen nås innan det förväntade antalet byte har lästs. |
| ObjectDisposedException | Kastas om källströmmen har frigjorts. |

### Se även

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## FromZstandard(string) {#fromzstandard_1}

Extraherar angivet Zstandard-arkiv och skapar [`TarArchive`](../) från den extraherade datan.

Viktigt: Zstandard-arkivet extraheras helt inom denna metod, dess innehåll behålls internt. Var medveten om minnesanvändning.

```csharp
public static TarArchive FromZstandard(string path)
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
| IOException | Zstandard-strömmen är skadad eller kan inte läsas. |
| InvalidDataException | Data är skadad. |
| EndOfStreamException | Kastas när slutet av strömmen nås innan det förväntade antalet byte har lästs. |

### Se även

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


