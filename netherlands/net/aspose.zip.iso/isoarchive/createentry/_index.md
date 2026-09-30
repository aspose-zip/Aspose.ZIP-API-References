---
title: "IsoArchive.CreateEntry"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "IsoArchive-methode. Voegt een bestand toe aan het ISO‑image."
type: docs
weight: 40
url: /nl/net/aspose.zip.iso/isoarchive/createentry/
---
## CreateEntry(string, string) {#createentry_2}

Voegt een bestand toe aan het ISO‑beeld.

```csharp
public IsoEntry CreateEntry(string name, string filePath)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| name | String | Pad van het bestand in de ISO. |
| filePath | String | Pad van het bestand. |

### Retourwaarde

De ISO-entry is samengesteld.

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ArgumentNullException | Het *filePath* is null. |
| ArgumentException | Het *filePath* is leeg, bevat alleen witruimtes, of bevat ongeldige tekens. |
| UnauthorizedAccessException | Toegang tot bestand *filePath* is geweigerd. |
| PathTooLongException | Het opgegeven *filePath* overschrijdt de systeemgedefinieerde maximale lengte. Bijvoorbeeld, op Windows-platformen moeten paden korter zijn dan 248 tekens, en bestandsnamen korter dan 260 tekens. |
| NotSupportedException | Bestand op *filePath* bevat een dubbele punt (:) in het midden van de tekenreeks. |
| IOException | Er trad een I/O-fout op tijdens het openen van het bestand. |
| ObjectDisposedException | Archief is verwijderd en kan niet worden gebruikt. |
| DirectoryNotFoundException | Het opgegeven pad is ongeldig, (bijvoorbeeld, het bevindt zich op een niet-toegewezen station). |
| FileNotFoundException | Het bestand opgegeven in *filePath* is niet gevonden. |
| InvalidOperationException | Het archief bevindt zich niet in bewerkingsmodus. |

### Zie ook

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream) {#createentry_1}

Voegt een bestand toe aan het ISO‑beeld.

```csharp
public IsoEntry CreateEntry(string name, Stream source)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| name | String | Pad van het bestand in de ISO. |
| bron | Stream | Stream die de bestandsgegevens bevat. |

### Retourwaarde

De ISO-entry is samengesteld.

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ObjectDisposedException | Archief is verwijderd en kan niet worden gebruikt. |
| ArgumentNullException | Wordt opgegooid wanneer een *name* of *source* null is. |
| InvalidOperationException | Het archief bevindt zich niet in bewerkingsmodus. |

### Zie ook

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string) {#createentry}

Voegt een bestand toe aan het ISO‑beeld.

```csharp
public IsoEntry CreateEntry(string name)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| name | String | Pad van de map in de ISO. |

### Retourwaarde

De ISO-entry is samengesteld.

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ArgumentNullException | `name` is null of leeg. |
| InvalidOperationException | Het archief is geopend voor extractie. |
| ObjectDisposedException | Archief is verwijderd en kan niet worden gebruikt. |

### Zie ook

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


