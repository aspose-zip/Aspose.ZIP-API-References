---
title: SharArchive.CreateEntries
second_title: Aspose.ZIP för .NET API-referens
description: SharArchive metod. Lägger till alla filer och kataloger i arkivet rekursivt i den angivna katalogen.
type: docs
weight: 30
url: /sv/net/aspose.zip.shar/shararchive/createentries/
---
## CreateEntries(string, bool) {#createentries_1}

Lägger till alla filer och kataloger i arkivet rekursivt i den angivna katalogen.

```csharp
public SharArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceDirectory | String | Katalog att komprimera. |
| includeRootDirectory | Boolean | Anger om själva rotkatalogen ska inkluderas eller inte. |

### Returvärde

Shar-inträdesinstans.

### Undantag

| undantag | skick |
| --- | --- |
| ArgumentNullException | *sourceDirectory* är inget. |
| SecurityException | Den som ringer har inte den behörighet som krävs för att få åtkomst*sourceDirectory*. |
| ArgumentException | *sourceDirectory* innehåller ogiltiga tecken som ", &lt;, &gt; eller &#x7C;. |
| PathTooLongException | Den angivna sökvägen, filnamnet eller båda överskrider den systemdefinierade maximala längden. Till exempel, på Windows-baserade plattformar måste sökvägar vara mindre än 248 tecken och filnamn måste vara mindre än 260 tecken. Den angivna sökvägen, filnamnet eller båda är för långa. |
| IOException | *sourceDirectory* står för en fil, inte för en katalog. |

### Exempel

```csharp
using (FileStream sharFile = File.Open("archive.shar", FileMode.Create))
{
    using (var archive = new SharArchive())
    {
        archive.CreateEntries("C:\folder", false);
        archive.Save(sharFile);
    }
}
```

### Se även

* class [SharArchive](../)
* namnutrymme [Aspose.Zip.Shar](../../shararchive/)
* hopsättning [Aspose.Zip](../../../)

---

## CreateEntries(DirectoryInfo, bool) {#createentries}

Lägger till alla filer och kataloger i arkivet rekursivt i den angivna katalogen.

```csharp
public SharArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| directory | DirectoryInfo | Katalog att komprimera. |
| includeRootDirectory | Boolean | Anger om själva rotkatalogen ska inkluderas eller inte. |

### Returvärde

Shar-inträdesinstans.

### Undantag

| undantag | skick |
| --- | --- |
| ArgumentNullException | *directory* är inget. |
| SecurityException | Den som ringer har inte den behörighet som krävs för att få åtkomst*directory*. |
| IOException | *directory* står för en fil, inte för en katalog. |

### Exempel

```csharp
using (FileStream sharFile = File.Open("archive.shar", FileMode.Create))
{
    using (var archive = new SharArchive())
    {
        archive.CreateEntries(new DirectoryInfo("C:\folder"), false);
        archive.Save(sharFile);
    }
}
```

### Se även

* class [SharArchive](../)
* namnutrymme [Aspose.Zip.Shar](../../shararchive/)
* hopsättning [Aspose.Zip](../../../)


