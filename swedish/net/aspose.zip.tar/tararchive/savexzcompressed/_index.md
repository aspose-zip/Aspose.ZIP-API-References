---
title: TarArchive.SaveXzCompressed
second_title: Aspose.ZIP för .NET API-referens
description: TarArchive metod. Sparar arkiv till strömmen med xzkomprimering.
type: docs
weight: 150
url: /sv/net/aspose.zip.tar/tararchive/savexzcompressed/
---
## SaveXzCompressed(Stream, TarFormat?, XzArchiveSettings) {#savexzcompressed}

Sparar arkiv till strömmen med xz-komprimering.

```csharp
public void SaveXzCompressed(Stream output, TarFormat? format = default, 
    XzArchiveSettings settings = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| output | Stream | Destinationsström. |
| format | Nullable`1 | Definierar tjärhuvudformat. Nullvärde kommer att behandlas som USTar när det är möjligt. |
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
using (FileStream result = File.OpenWrite("result.tar.xz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveXzCompressed(result);
        }
    }
}
```

### Se även

* enum [TarFormat](../../tarformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [TarArchive](../)
* namnutrymme [Aspose.Zip.Tar](../../tararchive/)
* hopsättning [Aspose.Zip](../../../)

---

## SaveXzCompressed(string, TarFormat?, XzArchiveSettings) {#savexzcompressed_1}

Sparar arkiv till sökvägen för sökväg med xz-komprimering.

```csharp
public void SaveXzCompressed(string path, TarFormat? format = default, 
    XzArchiveSettings settings = null)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| path | String | Sökvägen till arkivet som ska skapas. Om det angivna filnamnet pekar på en befintlig fil kommer den att skrivas över. |
| format | Nullable`1 | Definierar tjärhuvudformat. Nullvärde kommer att behandlas som USTar när det är möjligt. |
| settings | XzArchiveSettings | Uppsättning av inställningsspecifika xz-arkiv: ordbokstorlek, blockstorlek, kontrolltyp. |

### Exempel

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveXzCompressed("result.tar.xz");
    }
}
```

### Se även

* enum [TarFormat](../../tarformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [TarArchive](../)
* namnutrymme [Aspose.Zip.Tar](../../tararchive/)
* hopsättning [Aspose.Zip](../../../)


