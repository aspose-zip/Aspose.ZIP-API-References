---
title: TarArchive.SaveGzipped
second_title: Aspose.ZIP för .NET API-referens
description: TarArchive metod. Sparar arkiv i strömmen med gzipkomprimering.
type: docs
weight: 130
url: /sv/net/aspose.zip.tar/tararchive/savegzipped/
---
## SaveGzipped(Stream, TarFormat?) {#savegzipped}

Sparar arkiv i strömmen med gzip-komprimering.

```csharp
public void SaveGzipped(Stream output, TarFormat? format = default)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| output | Stream | Destinationsström. |
| format | Nullable`1 | Definierar tjärhuvudformat. Nullvärde kommer att behandlas som USTar när det är möjligt. |

### Undantag

| undantag | skick |
| --- | --- |
| ArgumentNullException | *output* är inget. |
| ArgumentException | *output* är inte skrivbar. |

### Anmärkningar

*output*måste vara skrivbar.

### Exempel

```csharp
using (FileStream result = File.OpenWrite("result.tar.gz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveGzipped(result);
        }
    }
}
```

### Se även

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* namnutrymme [Aspose.Zip.Tar](../../tararchive/)
* hopsättning [Aspose.Zip](../../../)

---

## SaveGzipped(string, TarFormat?) {#savegzipped_1}

Sparar arkiv till filen efter sökväg med gzip-komprimering.

```csharp
public void SaveGzipped(string path, TarFormat? format = default)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| path | String | Sökvägen till arkivet som ska skapas. Om det angivna filnamnet pekar på en befintlig fil kommer den att skrivas över. |
| format | Nullable`1 | Definierar tjärhuvudformat. Nullvärde kommer att behandlas som USTar när det är möjligt. |

### Exempel

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveGzipped("result.tar.gz");
    }
}
```

### Se även

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* namnutrymme [Aspose.Zip.Tar](../../tararchive/)
* hopsättning [Aspose.Zip](../../../)


