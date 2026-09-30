---
title: "UueArchive.Extract"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "UueArchive-methode. Extraheert het archief naar de opgegeven stream"
type: docs
weight: 40
url: /nl/net/aspose.zip.uue/uuearchive/extract/
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
| ObjectDisposedException | Archief is verwijderd en kan niet worden gebruikt. |
| ArgumentException | *destination* ondersteunt geen schrijven. |

## Voorbeelden

```csharp
using (var archive = new UueArchive("archive.uue"))
{
     archive.Extract(httpResponseStream);
}
```

### Zie ook

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

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

Info van het geëxtraheerde bestand.

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ObjectDisposedException | Archief is verwijderd en kan niet worden gebruikt. |
| ArgumentNullException | *path* is null. |
| SecurityException | De aanroeper heeft niet de vereiste toestemming om toegang te krijgen. |
| ArgumentException | Het *path* is leeg, bevat alleen witruimtes, of bevat ongeldige tekens. |
| UnauthorizedAccessException | Toegang tot bestand *path* is geweigerd. |
| PathTooLongException | Het opgegeven *path*, bestandsnaam, of beide overschrijden de systeemgedefinieerde maximale lengte. Bijvoorbeeld, op Windows-platformen moeten paden korter zijn dan 248 tekens, en bestandsnamen korter dan 260 tekens. |
| NotSupportedException | Bestand op *path* bevat een dubbele punt (:) in het midden van de tekenreeks. |
| FileNotFoundException | Het bestand is niet gevonden. |
| DirectoryNotFoundException | Het opgegeven pad is ongeldig, bijvoorbeeld omdat het zich op een niet-toegewezen station bevindt. |
| IOException | Het bestand is al geopend. |
| InvalidDataException | Wordt gegooid wanneer de gegevens ongeldig of beschadigd zijn. |

### Zie ook

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


