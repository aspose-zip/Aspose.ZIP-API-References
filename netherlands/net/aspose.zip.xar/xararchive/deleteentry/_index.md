---
title: "XarArchive.DeleteEntry"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "XarArchive-methode. Verwijdert de eerste voorkoming van een specifieke vermelding uit de vermeldinglijst."
type: docs
weight: 50
url: /nl/net/aspose.zip.xar/xararchive/deleteentry/
---
## XarArchive.DeleteEntry method

Verwijdert de eerste voorkoming van een specifieke vermelding uit de vermeldinglijst.

```csharp
public XarArchive DeleteEntry(XarEntry entry)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| item | XarEntry | De vermelding die verwijderd moet worden uit de vermeldinglijst. |

### Retourwaarde

Xar entry instantie.

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ArgumentNullException | *entry* is null. |
| ObjectDisposedException | Archief is verwijderd en kan niet worden gebruikt. |
| InvalidOperationException | Het archief is niet geopend voor extractie. |

## Voorbeelden

Hier volgt hoe u alle vermeldingen kunt verwijderen behalve de laatste:

```csharp
using (var archive = new XarArchive("archive.xar"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries.FirstOrDefault());
    archive.Save(outputXarFile);
}
```

### Zie ook

* class [XarEntry](../../xarentry/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


