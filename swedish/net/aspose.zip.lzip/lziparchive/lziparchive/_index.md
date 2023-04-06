---
title: LzipArchive.LzipArchive
second_title: Aspose.ZIP för .NET API-referens
description: LzipArchive byggare. Initierar en ny instans avLzipArchive .
type: docs
weight: 10
url: /sv/net/aspose.zip.lzip/lziparchive/lziparchive/
---
## LzipArchive(LzipArchiveSettings) {#constructor}

Initierar en ny instans av[`LzipArchive`](../) .

```csharp
public LzipArchive(LzipArchiveSettings settings = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| settings | LzipArchiveSettings | Inställning av särskilt lzip-arkiv med definition av ordboksstorlek. |

### Se även

* class [LzipArchiveSettings](../../lziparchivesettings/)
* class [LzipArchive](../)
* namnutrymme [Aspose.Zip.Lzip](../../lziparchive/)
* hopsättning [Aspose.Zip](../../../)

---

## LzipArchive(Stream) {#constructor_1}

Initierar en ny instans av[`LzipArchive`](../) klass förberedd för dekomprimering.

```csharp
public LzipArchive(Stream sourceStream)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceStream | Stream | Källan till arkivet. |

### Undantag

| undantag | skick |
| --- | --- |
| ArgumentException | *sourceStream* är inte sökbar. |
| ArgumentNullException | *sourceStream* är inget. |
| InvalidDataException | Rubriker matchar inte lzip-typen av arkiv. |

### Anmärkningar

Denna konstruktor dekomprimerar inte. Ser[`Extract`](../extract/) metod för dekomprimering.

### Se även

* class [LzipArchive](../)
* namnutrymme [Aspose.Zip.Lzip](../../lziparchive/)
* hopsättning [Aspose.Zip](../../../)

---

## LzipArchive(string) {#constructor_2}

Initierar en ny instans av[`LzipArchive`](../) klass förberedd för dekomprimering.

```csharp
public LzipArchive(string path)
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
| InvalidDataException | Rubriker matchar inte lzip-typen av arkiv. |

### Anmärkningar

Denna konstruktor dekomprimerar inte. Ser[`Extract`](../extract/) metod för dekomprimering.

### Exempel

```csharp
using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
{
    using (var archive = new LzipArchive(sourceLzipFile))
    {
         archive.Extract(extractedFile);
       }
   }
```

### Se även

* class [LzipArchive](../)
* namnutrymme [Aspose.Zip.Lzip](../../lziparchive/)
* hopsättning [Aspose.Zip](../../../)


