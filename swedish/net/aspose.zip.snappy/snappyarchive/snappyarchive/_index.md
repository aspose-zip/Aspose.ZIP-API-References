---
title: SnappyArchive.SnappyArchive
second_title: Aspose.ZIP för .NET API-referens
description: SnappyArchive byggare. Initierar en ny instans avSnappyArchive klass förberedd för komprimering.
type: docs
weight: 10
url: /sv/net/aspose.zip.snappy/snappyarchive/snappyarchive/
---
## SnappyArchive() {#constructor}

Initierar en ny instans av[`SnappyArchive`](../) klass förberedd för komprimering.

```csharp
public SnappyArchive()
```

### Exempel

Följande exempel visar hur man komprimerar en fil.

```csharp
using (SnappyArchive archive = new SnappyArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.snapy");
}
```

### Se även

* class [SnappyArchive](../)
* namnutrymme [Aspose.Zip.Snappy](../../snappyarchive/)
* hopsättning [Aspose.Zip](../../../)

---

## SnappyArchive(Stream) {#constructor_1}

Initierar en ny instans av[`SnappyArchive`](../) klass förberedd för dekomprimering.

```csharp
public SnappyArchive(Stream source)
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

* class [SnappyArchive](../)
* namnutrymme [Aspose.Zip.Snappy](../../snappyarchive/)
* hopsättning [Aspose.Zip](../../../)

---

## SnappyArchive(string) {#constructor_2}

Initierar en ny instans av[`SnappyArchive`](../) klass förberedd för dekomprimering.

```csharp
public SnappyArchive(string path)
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
    using (var archive = new SnappyArchive(sourceSnappyFile))
    {
         archive.Extract(extractedFile);
    }
   }
```

### Se även

* class [SnappyArchive](../)
* namnutrymme [Aspose.Zip.Snappy](../../snappyarchive/)
* hopsättning [Aspose.Zip](../../../)


