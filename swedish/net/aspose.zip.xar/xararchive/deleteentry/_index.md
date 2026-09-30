---
title: "XarArchive.DeleteEntry"
second_title: "Aspose.ZIP för .NET API-referens"
description: "XarArchive metod. Tar bort den första förekomsten av en specifik post från postlistan"
type: docs
weight: 50
url: /sv/net/aspose.zip.xar/xararchive/deleteentry/
---
## XarArchive.DeleteEntry method

Tar bort den första förekomsten av en specifik post från postlistan.

```csharp
public XarArchive DeleteEntry(XarEntry entry)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| post | XarEntry | Posten att ta bort från postlistan. |

### Returvärde

Xar-objektinstans.

### Undantag

| undantag | villkor |
| --- | --- |
| ArgumentNullException | *entry* är null. |
| ObjectDisposedException | Arkivet har frigjorts och kan inte användas. |
| InvalidOperationException | Arkivet är inte öppnat för extraktion. |

## Exempel

Här är hur du kan ta bort alla poster förutom den sista:

```csharp
using (var archive = new XarArchive("archive.xar"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries.FirstOrDefault());
    archive.Save(outputXarFile);
}
```

### Se även

* class [XarEntry](../../xarentry/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


