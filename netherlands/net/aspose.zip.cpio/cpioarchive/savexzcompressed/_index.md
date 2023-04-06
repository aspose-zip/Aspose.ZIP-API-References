---
title: CpioArchive.SaveXzCompressed
second_title: Aspose.ZIP voor .NET API-referentie
description: CpioArchive methode. Slaat archief op in de stream met xzcompressie.
type: docs
weight: 100
url: /nl/net/aspose.zip.cpio/cpioarchive/savexzcompressed/
---
## SaveXzCompressed(Stream, CpioFormat, XzArchiveSettings) {#savexzcompressed}

Slaat archief op in de stream met xz-compressie.

```csharp
public void SaveXzCompressed(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii, 
    XzArchiveSettings settings = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| output | Stream | Bestemmingsstroom. |
| cpioFormat | CpioFormat | Definieert de indeling van de cpio-header. |
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

### Zie ook

* enum [CpioFormat](../../cpioformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [CpioArchive](../)
* naamruimte [Aspose.Zip.Cpio](../../cpioarchive/)
* montage [Aspose.Zip](../../../)

---

## SaveXzCompressed(string, CpioFormat, XzArchiveSettings) {#savexzcompressed_1}

Slaat archief pad voor pad op met xz-compressie.

```csharp
public void SaveXzCompressed(string path, CpioFormat cpioFormat = CpioFormat.OldAscii, 
    XzArchiveSettings settings = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | String | Het pad van het aan te maken archief. Als de opgegeven bestandsnaam naar een bestaand bestand verwijst, wordt dit overschreven. |
| cpioFormat | CpioFormat | Definieert de indeling van de cpio-header. |
| settings | XzArchiveSettings | Set instellingen specifiek xz-archief: woordenboekgrootte, blokgrootte, controletype. |

### Voorbeelden

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

### Zie ook

* enum [CpioFormat](../../cpioformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [CpioArchive](../)
* naamruimte [Aspose.Zip.Cpio](../../cpioarchive/)
* montage [Aspose.Zip](../../../)


