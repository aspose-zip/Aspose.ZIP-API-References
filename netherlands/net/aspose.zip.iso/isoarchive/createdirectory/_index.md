---
title: "IsoArchive.CreateDirectory"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "IsoArchive-methode. Voegt een map toe aan het ISO-beeld"
type: docs
weight: 30
url: /nl/net/aspose.zip.iso/isoarchive/createdirectory/
---
## IsoArchive.CreateDirectory method

Voegt een map toe aan het ISO‑beeld.

```csharp
public IsoEntry CreateDirectory(string name)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| name | String | Pad van de map in de ISO. |

### Retourwaarde

De ISO-entry is samengesteld.

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| InvalidOperationException | Het archief is geopend voor extractie. |
| ArgumentNullException | `name` is null of leeg. |
| ObjectDisposedException | Archief is verwijderd en kan niet worden gebruikt. |

### Zie ook

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


