---
title: XzArchiveSettings.XzArchiveSettings
second_title: Aspose.ZIP voor .NET API-referentie
description: XzArchiveSettings constructeur. Initialiseert een nieuw exemplaar van hetXzArchiveSettings klasse met enkele LZMA2compressie.
type: docs
weight: 10
url: /nl/net/aspose.zip.xz.settings/xzarchivesettings/xzarchivesettings/
---
## XzArchiveSettings() {#constructor}

Initialiseert een nieuw exemplaar van het[`XzArchiveSettings`](../) klasse met enkele LZMA2-compressie.

```csharp
public XzArchiveSettings()
```

### Opmerkingen

Standaard woordenboek in LZMA2 filtergrootte is gelijk aan 16 megabyte, standaard blokgrootte is gelijk aan 64 megabytes, standaard controlesomtype is CRC32.

### Zie ook

* class [XzArchiveSettings](../)
* naamruimte [Aspose.Zip.Xz.Settings](../../xzarchivesettings/)
* montage [Aspose.Zip](../../../)

---

## XzArchiveSettings(XzFilterSettings[], long, XzCheckType) {#constructor_1}

Initialiseert een nieuw exemplaar van het[`XzArchiveSettings`](../) klasse met aangepaste parameters.

```csharp
public XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| filters | XzFilterSettings[] | Filters (compressors) die opeenvolgend moeten worden toegepast om te creëren[`XzArchive`](../../../aspose.zip.xz/xzarchive/) . Het kan zowel single zijn[`XzLZMA2FilterSettings`](../../xzlzma2filtersettings/) of paar[`XzBcjX86FilterSettings`](../../xzbcjx86filtersettings/) En[`XzLZMA2FilterSettings`](../../xzlzma2filtersettings/) |
| blockSize | Int64 | Grootte xz archiefblok. |
| checkType | XzCheckType | Type controlesomberekening voor niet-gecomprimeerde gegevens. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentOutOfRangeException | *blockSize* is negatief. |
| ArgumentNullException | *filters* is niets |
| ArgumentException | *filters* heeft minder dan één of meer dan twee filters, of het laatste filter niet[`XzLZMA2FilterSettings`](../../xzlzma2filtersettings/). |

### Voorbeelden

```csharp
using (FileStream xzFile = File.Open("archive.xz", FileMode.Create))
{
    XzLZMA2FilterSettings filter = new XzLZMA2FilterSettings(5242880);
    XzArchiveSettings settings = new XzArchiveSettings(new XzFilterSettings[] {filter}, 10485760, XzCheckType.Crc32);
    using (var archive = new XzArchive(settings))
    {
        archive.SetSource("data.bin");
        archive.Save(xzFile);
     }
}
```

### Zie ook

* class [XzFilterSettings](../../xzfiltersettings/)
* enum [XzCheckType](../../xzchecktype/)
* class [XzArchiveSettings](../)
* naamruimte [Aspose.Zip.Xz.Settings](../../xzarchivesettings/)
* montage [Aspose.Zip](../../../)


