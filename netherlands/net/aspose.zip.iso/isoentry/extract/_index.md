---
title: "IsoEntry.Extract"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "IsoEntry methode. Extraheert de entry naar het bestandssysteem via het opgegeven pad"
type: docs
weight: 50
url: /nl/net/aspose.zip.iso/isoentry/extract/
---
## Extract(string) {#extract}

Extraheert het item naar het bestandssysteem op het opgegeven pad.

```csharp
public FileInfo Extract(string path)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pad | String | Het pad naar het bestemmingsbestand. Als het bestand al bestaat, wordt het overschreven. |

### Retourwaarde

FileInfo‑instantie die de geëxtraheerde gegevens bevat.

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ArgumentNullException | *path* is null. |
| SecurityException | De aanroeper heeft niet de vereiste toestemming om toegang te krijgen. |
| ArgumentException | Het *path* is leeg, bevat alleen witruimtes, of bevat ongeldige tekens. |
| UnauthorizedAccessException | Toegang tot bestand *path* is geweigerd. |
| PathTooLongException | Het opgegeven *path*, bestandsnaam, of beide overschrijden de systeemgedefinieerde maximale lengte. Bijvoorbeeld, op Windows-platformen moeten paden korter zijn dan 248 tekens, en bestandsnamen korter dan 260 tekens. |
| NotSupportedException | Bestand op *path* bevat een dubbele punt (:) in het midden van de tekenreeks. |
| FileNotFoundException | Het bestand is niet gevonden. |
| DirectoryNotFoundException | Het opgegeven pad is ongeldig, bijvoorbeeld omdat het zich op een niet-toegewezen station bevindt. |
| IOException | Het bestand is al geopend. |
| InvalidOperationException | Archiefkoppen en service‑informatie zijn niet gelezen. |

### Zie ook

* class [IsoEntry](../)
* namespace [Aspose.Zip.Iso](../../isoentry/)
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
| NotSupportedException | Wordt opgegooid als de entry geen bestand vertegenwoordigt. |
| ArgumentException | De opgegeven stream ondersteunt geen schrijven. |

### Zie ook

* class [IsoEntry](../)
* namespace [Aspose.Zip.Iso](../../isoentry/)
* assembly [Aspose.Zip](../../../)


