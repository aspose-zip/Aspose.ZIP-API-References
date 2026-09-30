---
title: "AppleArchiveEntry.Extract"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "AppleArchiveEntry methode. Extraheert het item naar het bestandssysteem met het opgegeven pad"
type: docs
weight: 50
url: /nl/net/aspose.zip.apple/applearchiveentry/extract/
---
## Extract(string) {#extract}

Extraheert het item naar het bestandssysteem op het opgegeven pad.

```csharp
public FileInfo Extract(string path)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pad | String | Het pad naar het bestemmingsbestand. Als het bestand al bestaat, wordt het overschreven. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| InvalidDataException | De checksum of digest die voor het item is opgeslagen komt niet overeen met de geëxtraheerde gegevens. |
| InvalidOperationException | Het item behoort tot een archief dat is voorbereid voor compositie, of de itemgegevens kunnen niet worden geopend vanuit een niet-zoekbare archiefstroom. |
| NotSupportedException | Het item behoort tot een solide Apple-archief of gebruikt een niet-ondersteunde compressiemethode. |
| ObjectDisposedException | De bronstroom is verwijderd. |
| IOException | Er treedt een I/O-fout op. |

### Zie ook

* class [AppleArchiveEntry](../)
* namespace [Aspose.Zip.Apple](../../applearchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

Extraheert het item naar de opgegeven stream.

```csharp
public void Extract(Stream destination)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| bestemming | Stream | Bestemmingsstream. Moet schrijfbaar zijn. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ArgumentNullException | *destination* is `null`. |
| ArgumentException | *destination* ondersteunt geen schrijven. |
| InvalidDataException | De checksum of digest die voor het item is opgeslagen komt niet overeen met de geëxtraheerde gegevens. |
| InvalidOperationException | Het item behoort tot een archief dat is voorbereid voor compositie, of de itemgegevens kunnen niet worden geopend vanuit een niet-zoekbare archiefstroom. |
| NotSupportedException | Het item behoort tot een solide Apple-archief of gebruikt een niet-ondersteunde compressiemethode. |
| ObjectDisposedException | De bronstroom is verwijderd. |
| IOException | Er treedt een I/O-fout op. |

### Zie ook

* class [AppleArchiveEntry](../)
* namespace [Aspose.Zip.Apple](../../applearchiveentry/)
* assembly [Aspose.Zip](../../../)


