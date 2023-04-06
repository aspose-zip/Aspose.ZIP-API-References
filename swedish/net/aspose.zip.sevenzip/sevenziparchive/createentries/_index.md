---
title: SevenZipArchive.CreateEntries
second_title: Aspose.ZIP för .NET API-referens
description: SevenZipArchive metod. Lägger till alla filer och kataloger i arkivet rekursivt i den angivna katalogen.
type: docs
weight: 40
url: /sv/net/aspose.zip.sevenzip/sevenziparchive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

Lägger till alla filer och kataloger i arkivet rekursivt i den angivna katalogen.

```csharp
public SevenZipArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| directory | DirectoryInfo | Katalog att komprimera. |
| includeRootDirectory | Boolean | Anger om själva rotkatalogen ska inkluderas eller inte. |

### Returvärde

Arkivet med sammansatta poster.

### Undantag

| undantag | skick |
| --- | --- |
| DirectoryNotFoundException | Vägen till*directory* är ogiltigt, som att vara på en omappad enhet. |
| SecurityException | Den som ringer har inte den behörighet som krävs för att få åtkomst*directory*. |

### Exempel

```csharp
using (SevenZipArchive archive = new SevenZipArchive())
{
    DirectoryInfo folder = new DirectoryInfo("C:\folder");
    archive.CreateEntries(folder);
    archive.Save("folder.7z");
}
```

### Se även

* class [SevenZipArchive](../)
* namnutrymme [Aspose.Zip.SevenZip](../../sevenziparchive/)
* hopsättning [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

Lägger till alla filer och kataloger i arkivet rekursivt i den angivna katalogen.

```csharp
public SevenZipArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceDirectory | String | Katalog att komprimera. |
| includeRootDirectory | Boolean | Anger om själva rotkatalogen ska inkluderas eller inte. |

### Returvärde

Arkivet med sammansatta poster.

### Exempel

Komponera 7z-arkiv med LZMA2-komprimering.

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings())))
{
    archive.CreateEntries("C:\folder");
    archive.Save("folder.7z");
}
```

### Se även

* class [SevenZipArchive](../)
* namnutrymme [Aspose.Zip.SevenZip](../../sevenziparchive/)
* hopsättning [Aspose.Zip](../../../)


