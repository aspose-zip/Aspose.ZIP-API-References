---
title: CpioArchive.SaveGzipped
second_title: Aspose.ZIP för .NET API-referens
description: CpioArchive metod. Sparar arkiv i strömmen med gzipkomprimering.
type: docs
weight: 90
url: /sv/net/aspose.zip.cpio/cpioarchive/savegzipped/
---
## SaveGzipped(Stream, CpioFormat) {#savegzipped}

Sparar arkiv i strömmen med gzip-komprimering.

```csharp
public void SaveGzipped(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| output | Stream | Destinationsström. |
| cpioFormat | CpioFormat | Definierar cpio-huvudformat. |

### Undantag

| undantag | skick |
| --- | --- |
| ArgumentNullException | *output* är inget. |
| ArgumentException | *output* är inte skrivbar. |

### Anmärkningar

*output*måste vara skrivbar.

### Exempel

```csharp
using (FileStream result = File.OpenWrite("result.cpio.gz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveGzipped(result);
        }
    }
}
```

### Se även

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namnutrymme [Aspose.Zip.Cpio](../../cpioarchive/)
* hopsättning [Aspose.Zip](../../../)

---

## SaveGzipped(string, CpioFormat) {#savegzipped_1}

Sparar arkiv till filen efter sökväg med gzip-komprimering.

```csharp
public void SaveGzipped(string path, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| path | String | Sökvägen till arkivet som ska skapas. Om det angivna filnamnet pekar på en befintlig fil kommer den att skrivas över. |
| cpioFormat | CpioFormat | Definierar cpio-huvudformat. |

### Exempel

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveGzipped("result.cpio.gz");
    }
}
```

### Se även

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namnutrymme [Aspose.Zip.Cpio](../../cpioarchive/)
* hopsättning [Aspose.Zip](../../../)


