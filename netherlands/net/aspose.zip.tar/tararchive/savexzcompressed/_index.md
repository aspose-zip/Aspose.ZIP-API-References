---
title: TarArchive.SaveXzCompressed
second_title: Aspose.ZIP voor .NET API-referentie
description: TarArchive methode. Slaat archief op in de stream met xzcompressie.
type: docs
weight: 150
url: /nl/net/aspose.zip.tar/tararchive/savexzcompressed/
---
## SaveXzCompressed(Stream, TarFormat?, XzArchiveSettings) {#savexzcompressed}

Slaat archief op in de stream met xz-compressie.

```csharp
public void SaveXzCompressed(Stream output, TarFormat? format = default, 
    XzArchiveSettings settings = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| output | Stream | Bestemmingsstroom. |
| format | Nullable`1 | Definieert het formaat van de tar-koptekst. Null-waarde wordt indien mogelijk behandeld als UStar. |
| settings | XzArchiveSettings | Set instellingen specifiek xz-archief: woordenboekgrootte, blokgrootte, controletype. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentNullException | *output* is niets. |
| ArgumentException | *output* is niet beschrijfbaar. |

### Opmerkingen

*output*De stream moet beschrijfbaar zijn.

### Voorbeelden

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

### Zie ook

* enum [TarFormat](../../tarformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [TarArchive](../)
* naamruimte [Aspose.Zip.Tar](../../tararchive/)
* montage [Aspose.Zip](../../../)

---

## SaveXzCompressed(string, TarFormat?, XzArchiveSettings) {#savexzcompressed_1}

Slaat archief pad voor pad op met xz-compressie.

```csharp
public void SaveXzCompressed(string path, TarFormat? format = default, 
    XzArchiveSettings settings = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | String | Het pad van het aan te maken archief. Als de opgegeven bestandsnaam naar een bestaand bestand verwijst, wordt dit overschreven. |
| format | Nullable`1 | Definieert het formaat van de tar-koptekst. Null-waarde wordt indien mogelijk behandeld als UStar. |
| settings | XzArchiveSettings | Set instellingen specifiek xz-archief: woordenboekgrootte, blokgrootte, controletype. |

### Voorbeelden

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

### Zie ook

* enum [TarFormat](../../tarformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [TarArchive](../)
* naamruimte [Aspose.Zip.Tar](../../tararchive/)
* montage [Aspose.Zip](../../../)


