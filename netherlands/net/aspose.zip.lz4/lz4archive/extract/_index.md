---
title: "Lz4Archive.Extract"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "Lz4Archive-methode. Extraheert het archief naar het bestand op het pad"
type: docs
weight: 30
url: /nl/net/aspose.zip.lz4/lz4archive/extract/
---
## Extract(string) {#extract}

Extraheert het archief naar het bestand via pad.

```csharp
public FileInfo Extract(string path)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pad | String | Het pad naar het bestemmingsbestand. Als het bestand al bestaat, wordt het overschreven. |

### Retourwaarde

Info van een geëxtraheerd bestand.

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| EndOfStreamException | Bronstroom is te kort. |
| InvalidDataException | Verkeerde bytes gevonden tijdens het decoderen. |
| NotSupportedException | Deze LZ4-versie wordt niet ondersteund. |
| OperationCanceledException | In .NET Framework 4.0 en hoger: Wordt gegooid wanneer de extractie wordt geannuleerd via het opgegeven annulerings‑token. |
| ObjectDisposedException | Archief is verwijderd en kan niet worden gebruikt. |
| InvalidOperationException | Het archief is voorbereid op samenstelling. |

### Zie ook

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

Extraheert het archief naar de opgegeven stream.

```csharp
public void Extract(Stream destination)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| bestemming | Stream | Bestemmingsstream. Moet schrijfbaar zijn. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ArgumentException | *destination* ondersteunt geen schrijven. |
| EndOfStreamException | Bronstroom is te kort. |
| InvalidDataException | Verkeerde bytes gevonden tijdens het decoderen. |
| NotSupportedException | Deze LZ4-versie wordt niet ondersteund. |
| InvalidOperationException | Het archief is voorbereid op samenstelling. |
| OperationCanceledException | In .NET Framework 4.0 en hoger: Wordt gegooid wanneer de extractie wordt geannuleerd via het opgegeven annulerings‑token. |
| ObjectDisposedException | Archief is verwijderd en kan niet worden gebruikt. |

## Voorbeelden

```csharp
using (var archive = new Lz4Archive("archive.lz4"))
{
     archive.Extract(httpResponseStream);
}
```

### Zie ook

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


