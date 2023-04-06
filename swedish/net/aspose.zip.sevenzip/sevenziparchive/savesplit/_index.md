---
title: SevenZipArchive.SaveSplit
second_title: Aspose.ZIP för .NET API-referens
description: SevenZipArchive metod. Sparar arkiv med flera volymer i den tillhandahållna destinationskatalogen.
type: docs
weight: 90
url: /sv/net/aspose.zip.sevenzip/sevenziparchive/savesplit/
---
## SevenZipArchive.SaveSplit method

Sparar arkiv med flera volymer i den tillhandahållna destinationskatalogen.

```csharp
public void SaveSplit(string destinationDirectory, SplitSevenZipArchiveSaveOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| destinationDirectory | String | Sökvägen till katalogen där arkivsegmenten ska skapas. |
| options | SplitSevenZipArchiveSaveOptions | Alternativ för att spara arkiv, inklusive filnamn. |

### Undantag

| undantag | skick |
| --- | --- |
| InvalidOperationException | Detta arkiv öppnades från befintlig källa. |
| ArgumentNullException | *destinationDirectory* är inget. |
| SecurityException | Den som ringer har inte den behörighet som krävs för att komma åt telefonboken. |
| ArgumentException | *destinationDirectory* innehåller ogiltiga tecken som ", &gt;, &lt; eller &#x7C;. |
| PathTooLongException | Den angivna sökvägen överskrider den systemdefinierade maximala längden. |

### Anmärkningar

Denna metod består av flera (`n`) filer filnamn.7z.001, filnamn.7z.002, ..., filnamn.7z.(n).

Kan inte göra befintligt arkiv till flera volymer.

### Exempel

```csharp
using (SevenZipArchive archive = new SevenZipArchive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.SaveSplit(@"C:\Folder",  new SplitSevenZipArchiveSaveOptions("volume", 65536));
}
```

### Se även

* class [SplitSevenZipArchiveSaveOptions](../../../aspose.zip.saving/splitsevenziparchivesaveoptions/)
* class [SevenZipArchive](../)
* namnutrymme [Aspose.Zip.SevenZip](../../sevenziparchive/)
* hopsättning [Aspose.Zip](../../../)


