---
title: XarArchive.XarArchive
second_title: Aspose.ZIP för .NET API-referens
description: XarArchive byggare. Initierar en ny instans avXarArchive klass och komponerar poster lista kan extraheras från arkivet.
type: docs
weight: 10
url: /sv/net/aspose.zip.xar/xararchive/xararchive/
---
## XarArchive(Stream) {#constructor}

Initierar en ny instans av[`XarArchive`](../) klass och komponerar poster lista kan extraheras från arkivet.

```csharp
public XarArchive(Stream sourceStream)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceStream | Stream | Källan till arkivet. Det måste vara sökbart. |

### Undantag

| undantag | skick |
| --- | --- |
| ArgumentNullException | *sourceStream* är inget. |
| ArgumentException | *sourceStream* är inte sökbar. |
| InvalidDataException | *sourceStream* är inte giltigt xar-arkiv. |

### Anmärkningar

Denna konstruktor packar inte upp någon post. Ser[`Open`](../../xarfileentry/open/)metod för uppackning.

### Exempel

Följande exempel visar hur man extraherar alla poster till en katalog.

```csharp
using (var archive = new XarArchive(File.OpenRead("archive.xar")))
{
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Se även

* class [XarArchive](../)
* namnutrymme [Aspose.Zip.Xar](../../xararchive/)
* hopsättning [Aspose.Zip](../../../)

---

## XarArchive(string) {#constructor_1}

Initierar en ny instans av[`XarArchive`](../) klass och komponerar poster lista kan extraheras från arkivet.

```csharp
public XarArchive(string path)
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

Denna konstruktor packar inte upp någon post. Ser[`Open`](../../xarfileentry/open/)metod för uppackning.

### Exempel

Följande exempel visar hur man extraherar alla poster till en katalog.

```csharp
using (var archive = new XarArchive("archive.xar")) 
{
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Se även

* class [XarArchive](../)
* namnutrymme [Aspose.Zip.Xar](../../xararchive/)
* hopsättning [Aspose.Zip](../../../)


