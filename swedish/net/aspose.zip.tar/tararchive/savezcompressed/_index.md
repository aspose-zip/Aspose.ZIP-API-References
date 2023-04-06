---
title: TarArchive.SaveZCompressed
second_title: Aspose.ZIP för .NET API-referens
description: TarArchive metod. Sparar arkiv i strömmen med Zkomprimering.
type: docs
weight: 160
url: /sv/net/aspose.zip.tar/tararchive/savezcompressed/
---
## SaveZCompressed(Stream, TarFormat?) {#savezcompressed}

Sparar arkiv i strömmen med Z-komprimering.

```csharp
public void SaveZCompressed(Stream output, TarFormat? format = default)
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
using (FileStream result = File.OpenWrite("result.tar.Z"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveZCompressed(result);
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

## SaveZCompressed(string, TarFormat?) {#savezcompressed_1}

Sparar arkiv till sökvägen för sökväg med Z-komprimering.

```csharp
public void SaveZCompressed(string path, TarFormat? format = default)
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
        archive.SaveZCompressed("result.tar.Z");
    }
}
```

### Se även

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* namnutrymme [Aspose.Zip.Tar](../../tararchive/)
* hopsättning [Aspose.Zip](../../../)


