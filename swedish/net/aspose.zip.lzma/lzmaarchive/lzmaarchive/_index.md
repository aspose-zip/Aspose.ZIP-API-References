---
title: LzmaArchive.LzmaArchive
second_title: Aspose.ZIP för .NET API-referens
description: LzmaArchive byggare. Initierar en ny instans avLzmaArchive klass och komponerar arkivet i lzmaformat.
type: docs
weight: 10
url: /sv/net/aspose.zip.lzma/lzmaarchive/lzmaarchive/
---
## LzmaArchive(LzmaArchiveSettings) {#constructor}

Initierar en ny instans av[`LzmaArchive`](../) klass och komponerar arkivet i lzma-format.

```csharp
public LzmaArchive(LzmaArchiveSettings settings = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| settings | LzmaArchiveSettings | Uppsättning av inställningsspecifika lzma-arkiv. |

### Se även

* class [LzmaArchiveSettings](../../lzmaarchivesettings/)
* class [LzmaArchive](../)
* namnutrymme [Aspose.Zip.LZMA](../../lzmaarchive/)
* hopsättning [Aspose.Zip](../../../)

---

## LzmaArchive(Stream) {#constructor_1}

Initierar en ny instans av[`LzmaArchive`](../) klass förberedd för dekomprimering.

```csharp
public LzmaArchive(Stream source)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| source | Stream | Källan till arkivet. |

### Undantag

| undantag | skick |
| --- | --- |
| ArgumentException | *source* är inte sökbar. |
| ArgumentNullException | *source* är inget. |

### Anmärkningar

Denna konstruktor dekomprimerar inte. Ser[`Extract`](../extract/) metod för dekomprimering.

### Se även

* class [LzmaArchive](../)
* namnutrymme [Aspose.Zip.LZMA](../../lzmaarchive/)
* hopsättning [Aspose.Zip](../../../)

---

## LzmaArchive(string) {#constructor_2}

Initierar en ny instans av[`LzmaArchive`](../) klass förberedd för dekomprimering.

```csharp
public LzmaArchive(string path)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| path | String | Sökväg till källan till arkivet. |

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

Denna konstruktor dekomprimerar inte. Ser[`Extract`](../extract/) metod för dekomprimering.

### Exempel

```csharp
using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
{
    using (var archive = new LzmaArchive(sourceLzmaFile))
    {
         archive.Extract(extractedFile);
    }
   }
```

### Se även

* class [LzmaArchive](../)
* namnutrymme [Aspose.Zip.LZMA](../../lzmaarchive/)
* hopsättning [Aspose.Zip](../../../)


