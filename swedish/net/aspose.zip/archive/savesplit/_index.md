---
title: Archive.SaveSplit
second_title: Aspose.ZIP för .NET API-referens
description: Archive metod. Sparar arkiv med flera volymer i den tillhandahållna destinationskatalogen.
type: docs
weight: 100
url: /sv/net/aspose.zip/archive/savesplit/
---
## Archive.SaveSplit method

Sparar arkiv med flera volymer i den tillhandahållna destinationskatalogen.

```csharp
public void SaveSplit(string destinationDirectory, SplitArchiveSaveOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| destinationDirectory | String | Sökvägen till katalogen där arkivsegmenten ska skapas. |
| options | SplitArchiveSaveOptions | Alternativ för att spara arkiv, inklusive filnamn. |

### Undantag

| undantag | skick |
| --- | --- |
| InvalidOperationException | Detta arkiv öppnades från befintlig källa. |
| NotSupportedException | Detta arkiv är både komprimerat med XZ-metoden och krypterat. |
| ArgumentNullException | *destinationDirectory* är inget. |
| SecurityException | Den som ringer har inte den behörighet som krävs för att komma åt telefonboken. |
| ArgumentException | *destinationDirectory* innehåller ogiltiga tecken som ", &gt;, &lt; eller &#x7C;. |
| PathTooLongException | Den angivna sökvägen överskrider den systemdefinierade maximala längden. |

### Anmärkningar

Denna metod består av flera (`n`) filer filnamn.z01, filnamn.z02, ..., filnamn.z(n-1), filnamn.zip.

Kan inte göra befintligt arkiv till flera volymer.

### Exempel

```csharp
using (Archive archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.SaveSplit(@"C:\Folder",  new SplitArchiveSaveOptions("volume", 65536));
}
```

### Se även

* class [SplitArchiveSaveOptions](../../../aspose.zip.saving/splitarchivesaveoptions/)
* class [Archive](../)
* namnutrymme [Aspose.Zip](../../archive/)
* hopsättning [Aspose.Zip](../../../)


