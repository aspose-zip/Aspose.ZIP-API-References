---
title: CpioArchive.SaveXzCompressed
second_title: Aspose.ZIP för .NET API-referens
description: CpioArchive metod. Sparar arkiv till strömmen med xzkomprimering.
type: docs
weight: 100
url: /sv/net/aspose.zip.cpio/cpioarchive/savexzcompressed/
---
## SaveXzCompressed(Stream, CpioFormat, XzArchiveSettings) {#savexzcompressed}

Sparar arkiv till strömmen med xz-komprimering.

```csharp
public void SaveXzCompressed(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii, 
    XzArchiveSettings settings = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| output | Stream | Destinationsström. |
| cpioFormat | CpioFormat | Definierar cpio-huvudformat. |
| settings | XzArchiveSettings | Uppsättning av inställningsspecifika xz-arkiv: ordbokstorlek, blockstorlek, kontrolltyp. |

### Undantag

| undantag | skick |
| --- | --- |
| ArgumentNullException | *output* är inget. |
| ArgumentException | *output* är inte skrivbar. |

### Anmärkningar

*output*Strömmen måste vara skrivbar.

### Exempel

```csharp
using (FileStream result = File.OpenWrite("result.cpio.xz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveXzCompressed(result);
        }
    }
}
```

### Se även

* enum [CpioFormat](../../cpioformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [CpioArchive](../)
* namnutrymme [Aspose.Zip.Cpio](../../cpioarchive/)
* hopsättning [Aspose.Zip](../../../)

---

## SaveXzCompressed(string, CpioFormat, XzArchiveSettings) {#savexzcompressed_1}

Sparar arkiv till sökvägen för sökväg med xz-komprimering.

```csharp
public void SaveXzCompressed(string path, CpioFormat cpioFormat = CpioFormat.OldAscii, 
    XzArchiveSettings settings = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| path | String | Sökvägen till arkivet som ska skapas. Om det angivna filnamnet pekar på en befintlig fil kommer den att skrivas över. |
| cpioFormat | CpioFormat | Definierar cpio-huvudformat. |
| settings | XzArchiveSettings | Uppsättning av inställningsspecifika xz-arkiv: ordbokstorlek, blockstorlek, kontrolltyp. |

### Exempel

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveXzCompressed("result.cpio.xz");
    }
}
```

### Se även

* enum [CpioFormat](../../cpioformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [CpioArchive](../)
* namnutrymme [Aspose.Zip.Cpio](../../cpioarchive/)
* hopsättning [Aspose.Zip](../../../)


