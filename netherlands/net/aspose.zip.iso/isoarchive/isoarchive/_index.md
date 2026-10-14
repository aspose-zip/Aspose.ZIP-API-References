---
title: "IsoArchive.IsoArchive"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "IsoArchive constructor. Initialiseert een nieuw exemplaar van de IsoArchive-klasse en maakt een leeg ISO-archief aan voor het toevoegen van nieuwe bestanden en mappen."
type: docs
weight: 10
url: /nl/net/aspose.zip.iso/isoarchive/isoarchive/
---
## IsoArchive() {#constructor}

Initialiseert een nieuw exemplaar van de [`IsoArchive`](../)-klasse en maakt een leeg ISO-archief aan voor het toevoegen van nieuwe bestanden en mappen.

```csharp
public IsoArchive()
```

## Voorbeelden

Het volgende voorbeeld laat zien hoe je een nieuw leeg ISO-archief maakt en er bestanden aan toevoegt:

```csharp
// Maak een nieuw leeg ISO-archief
using(IsoArchive isoArchive = new IsoArchive())
{
    // Voeg bestanden toe aan het ISO-archief
    isoArchive.CreateEntry("example_file.txt", "path_to_file.txt");

    // Sla het ISO-archief op in een bestand
    isoArchive.Save("new_archive.iso");
}
```

### Zie ook

* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## IsoArchive(Stream, IsoLoadOptions) {#constructor_1}

Initialiseert een nieuw exemplaar van de [`IsoArchive`](../)-klasse en stelt een lijst met items samen die uit het archief kan worden geëxtraheerd.

```csharp
public IsoArchive(Stream sourceStream, IsoLoadOptions loadOptions = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| sourceStream | Stream | De bron van het archief. Deze moet doorzoekbaar zijn. |
| loadOptions | IsoLoadOptions | De opties om het archief mee te laden. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ArgumentNullException | *sourceStream* is null. |
| ArgumentException | *sourceStream* is niet doorzoekbaar. |
| InvalidDataException | *sourceStream* is geen geldig ISO-archief. |
| ObjectDisposedException | Wordt opgegooid als de bronstroom is verwijderd. |
| EndOfStreamException | Wordt opgegooid wanneer het einde van de stroom onverwacht wordt bereikt. |
| IOException | Er treedt een I/O-fout op. |
| NotSupportedException | De stroom ondersteunt geen lezen. |

## Opmerkingen

Deze constructor pakt geen enkel item uit.

## Voorbeelden

Het volgende voorbeeld laat zien hoe alle items naar een map worden geëxtraheerd.

```csharp
using (var archive = new IsoArchive(File.OpenRead("archive.iso")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Zie ook

* class [IsoLoadOptions](../../isoloadoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## IsoArchive(string, IsoLoadOptions) {#constructor_2}

Initialiseert een nieuw exemplaar van de [`IsoArchive`](../)-klasse en stelt een lijst met items samen die uit het archief kan worden geëxtraheerd.

```csharp
public IsoArchive(string path, IsoLoadOptions loadOptions = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pad | String | Het pad naar het archiefbestand. |
| loadOptions | IsoLoadOptions | De opties om het archief mee te laden. |

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
| EndOfStreamException | Het bestand is te kort. |
| InvalidDataException | Wordt gegooid wanneer de gegevens ongeldig of beschadigd zijn. |

## Opmerkingen

Deze constructor pakt geen enkel item uit.

## Voorbeelden

Het volgende voorbeeld laat zien hoe alle items naar een map worden geëxtraheerd.

```csharp
using (var archive = new IsoArchive("archive.iso")) 
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Zie ook

* class [IsoLoadOptions](../../isoloadoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


