---
title: "ArjArchive.ArjArchive"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "ArjArchive constructor. Initialiseert een nieuw exemplaar van de ArjArchive‑klasse en stelt een lijst met items samen die uit het archief kunnen worden geëxtraheerd"
type: docs
weight: 10
url: /nl/net/aspose.zip.arj/arjarchive/arjarchive/
---
## ArjArchive(Stream, ArjLoadOptions) {#constructor}

Initialiseert een nieuw exemplaar van de [`ArjArchive`](../)‑klasse en stelt een lijst met items samen die uit het archief kunnen worden geëxtraheerd.

```csharp
public ArjArchive(Stream extractionSource, ArjLoadOptions loadOptions = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| extractionSource | Stream | De bron van het archief. |
| loadOptions | ArjLoadOptions | Opties om een bestaand archief mee te laden. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ArgumentNullException | *extractionSource* is null. |
| ArgumentException | &gt;*extractionSource* ondersteunt geen zoeken. |
| InvalidDataException | Verkeerde handtekening voor archief. - of - Het bestand is geen ARJ‑archief. |
| EndOfStreamException | Wordt gegooid wanneer het einde van de stream wordt bereikt voordat alle headerbytes of naambytes zijn gelezen. |
| NotSupportedException | Het archief is beschadigd. |

## Opmerkingen

Deze constructor decompresseert geen enkel item. Zie de [`Extract`](../../arjentryplain/extract/) methode voor decompressie.

### Zie ook

* class [ArjLoadOptions](../../arjloadoptions/)
* class [ArjArchive](../)
* namespace [Aspose.Zip.Arj](../../arjarchive/)
* assembly [Aspose.Zip](../../../)

---

## ArjArchive(string, ArjLoadOptions) {#constructor_1}

Initialiseert een nieuw exemplaar van de [`ArjArchive`](../)‑klasse en stelt een lijst met items samen die uit het archief kunnen worden geëxtraheerd.

```csharp
public ArjArchive(string path, ArjLoadOptions loadOptions = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pad | String | Het pad naar het archiefbestand. |
| loadOptions | ArjLoadOptions | Opties om een bestaand archief mee te laden. |

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
| EndOfStreamException | Wordt gegooid wanneer het einde van de stream wordt bereikt voordat alle headerbytes of naambytes zijn gelezen. |
| InvalidDataException | Het ARJ‑magische getal is ongeldig of de headergrootte valt buiten het bereik. |

## Opmerkingen

Deze constructor pakt geen enkel item uit. Zie de [`Extract`](../../arjentryplain/extract/) methode voor decompressie.

## Voorbeelden

Het volgende voorbeeld laat zien hoe alle items naar een map worden geëxtraheerd.

```csharp
using (var archive = new ArjArchive("archive.arj")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Zie ook

* class [ArjLoadOptions](../../arjloadoptions/)
* class [ArjArchive](../)
* namespace [Aspose.Zip.Arj](../../arjarchive/)
* assembly [Aspose.Zip](../../../)


