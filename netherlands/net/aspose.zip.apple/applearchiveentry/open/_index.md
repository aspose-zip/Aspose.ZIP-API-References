---
title: "AppleArchiveEntry.Open"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "AppleArchiveEntry methode. Opent het item voor extractie en levert een stroom met de inhoud van het item"
type: docs
weight: 60
url: /nl/net/aspose.zip.apple/applearchiveentry/open/
---
## AppleArchiveEntry.Open method

Opent het item voor extractie en biedt een stream met de inhoud van het item.

```csharp
public Stream Open()
```

### Retourwaarde

Een leesbare stroom die de geëxtraheerde itemgegevens bevat.

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| NotSupportedException | Het item behoort tot een solide Apple-archief of gebruikt een niet-ondersteunde compressiemethode. |
| InvalidDataException | De checksum of digest die voor het item is opgeslagen komt niet overeen met de geëxtraheerde gegevens. |
| InvalidOperationException | Het item behoort tot een archief dat is voorbereid voor compositie, of de itemgegevens kunnen niet worden geopend vanuit een niet-zoekbare archiefstroom. |
| ObjectDisposedException | De bronstroom is verwijderd. |
| IOException | Er treedt een I/O-fout op. |

## Opmerkingen

Lees van de geretourneerde stroom om de oorspronkelijke iteminhoud te verkrijgen. Als het archief checksum-velden bevat, wordt de checksum geverifieerd terwijl de geretourneerde stroom wordt gelezen.

### Zie ook

* class [AppleArchiveEntry](../)
* namespace [Aspose.Zip.Apple](../../applearchiveentry/)
* assembly [Aspose.Zip](../../../)


