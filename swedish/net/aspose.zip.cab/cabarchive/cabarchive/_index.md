---
title: CabArchive.CabArchive
second_title: Aspose.ZIP för .NET API-referens
description: CabArchive byggare. Initierar en ny instans avCabArchive klass och komponerar poster lista kan extraheras från arkivet.
type: docs
weight: 10
url: /sv/net/aspose.zip.cab/cabarchive/cabarchive/
---
## CabArchive(Stream) {#constructor}

Initierar en ny instans av[`CabArchive`](../) klass och komponerar poster lista kan extraheras från arkivet.

```csharp
public CabArchive(Stream sourceStream)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceStream | Stream | Källan till arkivet. Det måste vara sökbart. |

### Undantag

| undantag | skick |
| --- | --- |
| ArgumentNullException | *sourceStream* är inget. |
| ArgumentException | *sourceStream* är inte sökbar. |
| InvalidDataException | *sourceStream* är inte giltigt hyttarkiv. |

### Anmärkningar

Denna konstruktor packar inte upp någon post. Ser[`Open`](../../cabentry/open/)metod för uppackning.

### Exempel

Följande exempel visar hur man extraherar alla poster till en katalog.

```csharp
using (var archive = new CabArchive(File.OpenRead("archive.cab")))
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Se även

* class [CabArchive](../)
* namnutrymme [Aspose.Zip.Cab](../../cabarchive/)
* hopsättning [Aspose.Zip](../../../)

---

## CabArchive(string) {#constructor_1}

Initierar en ny instans av[`CabArchive`](../) klass och komponerar poster lista kan extraheras från arkivet.

```csharp
public CabArchive(string path)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| path | String | Sökvägen till arkivfilen. |

### Undantag

| undantag | skick |
| --- | --- |
| ArgumentNullException | *path* är inget. |
| SecurityException | Den som ringer har inte den behörighet som krävs för att få åtkomst. |
| ArgumentException | De*path* är tom, innehåller bara blanksteg eller innehåller ogiltiga tecken. |
| UnauthorizedAccessException | Tillgång till fil*path* är nekad. |
| PathTooLongException | Den angivna*path*, filnamn eller båda överskrider den systemdefinierade maximala längden. Till exempel, på Windows-baserade plattformar måste sökvägar vara mindre än 248 tecken och filnamn måste vara mindre än 260 tecken. |
| NotSupportedException | Arkivera kl*path* innehåller ett kolon (:) i mitten av strängen. |

### Anmärkningar

Denna konstruktor packar inte upp någon post. Ser[`Open`](../../cabentry/open/)metod för uppackning.

### Exempel

Följande exempel visar hur man extraherar alla poster till en katalog.

```csharp
using (var archive = new CabArchive("archive.cab")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Se även

* class [CabArchive](../)
* namnutrymme [Aspose.Zip.Cab](../../cabarchive/)
* hopsättning [Aspose.Zip](../../../)


