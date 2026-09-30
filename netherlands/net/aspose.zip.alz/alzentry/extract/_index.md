---
title: "AlzEntry.Extract"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "AlzEntry methode. Extraheert het item naar het bestandssysteem via het opgegeven pad"
type: docs
weight: 60
url: /nl/net/aspose.zip.alz/alzentry/extract/
---
## Extract(string, string) {#extract}

Extraheert het item naar het bestandssysteem op het opgegeven pad.

```csharp
public FileInfo Extract(string path, string password = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pad | String | Het pad naar het bestemmingsbestand. Als het bestand al bestaat, wordt het overschreven. |
| wachtwoord | String | Optioneel wachtwoord voor decryptie. |

### Retourwaarde

De bestandsinfo van een samengesteld bestand.

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ArgumentNullException | *path* is null. |
| SecurityException | De aanroeper heeft niet de vereiste toestemming om toegang te krijgen. |
| ArgumentException | Het *path* is leeg, bevat alleen witruimtes, of bevat ongeldige tekens. |
| UnauthorizedAccessException | Toegang tot bestand *path* is geweigerd. |
| PathTooLongException | Het opgegeven *path*, bestandsnaam, of beide overschrijden de systeemgedefinieerde maximale lengte. Bijvoorbeeld, op Windows-platformen moeten paden korter zijn dan 248 tekens, en bestandsnamen korter dan 260 tekens. |
| NotSupportedException | Bestand op *path* bevat een dubbele punt (:) in het midden van de tekenreeks. |
| InvalidDataException | Het archief is beschadigd. |
| OperationCanceledException | In .NET Framework 4.0 en hoger: Wordt gegooid wanneer de extractie wordt geannuleerd via het opgegeven annulerings‑token. |
| ObjectDisposedException | Wordt opgegooid als de bronstroom is verwijderd. |
| FileNotFoundException | Het bestand is niet gevonden. |

## Voorbeelden

```csharp
using (var archive = new SevenZipArchive("archive.7z"))
{
    archive.Entries[0].Extract("data.bin");
}
```

### Zie ook

* class [AlzEntry](../)
* namespace [Aspose.Zip.Alz](../../alzentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream, string) {#extract_1}

Extraheert het item naar de opgegeven stream.

```csharp
public void Extract(Stream destination, string password = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| bestemming | Stream | Bestemmingsstream. Moet schrijfbaar zijn. |
| wachtwoord | String | Optioneel wachtwoord voor decryptie. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ArgumentException | *destination* ondersteunt geen schrijven. |
| InvalidOperationException | Het archief is niet geopend voor extractie. - of - Dit item is een map. |
| InvalidDataException | Onjuiste gegevens binnen het item. |
| OperationCanceledException | In .NET Framework 4.0 en hoger: Wordt gegooid wanneer de extractie wordt geannuleerd via het opgegeven annulerings‑token. |

## Voorbeelden

Extraheer een item van het ALZ‑archief met wachtwoord.

```csharp
using (var archive = new SevenZipArchive("archive.7z"))
{
    archive.Entries[0].Extract(httpResponseStream);
}
```

### Zie ook

* class [AlzEntry](../)
* namespace [Aspose.Zip.Alz](../../alzentry/)
* assembly [Aspose.Zip](../../../)


