---
title: "LhaArchiveEntry.Extract"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "LhaArchiveEntry-methode. Extraheert Lha-archiefitem naar een bestandssysteem via pad"
type: docs
weight: 60
url: /nl/net/aspose.zip.lha/lhaarchiveentry/extract/
---
## Extract(string) {#extract}

Extraheert Lha-archiefitem naar een bestandssysteem via pad.

```csharp
public FileSystemInfo Extract(string path)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pad | String | Pad naar het bestand dat de gedecomprimeerde gegevens zal opslaan. |

### Retourwaarde

FileSystemInfoInstance met uitgepakte gegevens.

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| InvalidOperationException | Archiefkoppen en service‑informatie zijn niet gelezen. |
| ArgumentNullException | *path* is null. |
| SecurityException | De aanroeper heeft niet de vereiste toestemming om toegang te krijgen. |
| ArgumentException | Het *path* is leeg, bevat alleen witruimtes, of bevat ongeldige tekens. |
| UnauthorizedAccessException | Toegang tot bestand *path* is geweigerd. |
| PathTooLongException | Het opgegeven *path*, bestandsnaam, of beide overschrijden de systeemgedefinieerde maximale lengte. Bijvoorbeeld, op Windows-platformen moeten paden korter zijn dan 248 tekens, en bestandsnamen korter dan 260 tekens. |
| NotSupportedException | Bestand op *path* bevat een dubbele punt (:) in het midden van de tekenreeks. |
| OperationCanceledException | In .NET Framework 4.0 en hoger: Wordt gegooid wanneer de extractie wordt geannuleerd via het opgegeven annulerings‑token. |
| ObjectDisposedException | Wordt opgegooid als de bronstroom is verwijderd. |
| InvalidDataException | Wordt gegooid wanneer de gegevens ongeldig of beschadigd zijn. |

## Voorbeelden

```csharp
using (FileStream lhaFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LhaArchive(lhaFile))
    {
        archive.Entries[0].Extract("extracted.bin");
    }
}
```

### Zie ook

* class [LhaArchiveEntry](../)
* namespace [Aspose.Zip.Lha](../../lhaarchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_2}

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
| ArgumentException | *destination* ondersteunt geen schrijven. |
| OperationCanceledException | In .NET Framework 4.0 en hoger: Wordt gegooid wanneer de extractie wordt geannuleerd via het opgegeven annulerings‑token. |
| ObjectDisposedException | Wordt opgegooid als de bronstroom is verwijderd. |
| InvalidDataException | Wordt gegooid wanneer de gegevens ongeldig of beschadigd zijn. |

## Opmerkingen

Doet niets voor mapitem.

### Zie ook

* class [LhaArchiveEntry](../)
* namespace [Aspose.Zip.Lha](../../lhaarchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

Extraheert Lha-archiefitem naar een bestand.

```csharp
public void Extract(FileInfo fileInfo)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fileInfo | FileInfo | FileInfo voor het opslaan van gedecomprimeerde gegevens. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| InvalidOperationException | Archiefkoppen en service‑informatie zijn niet gelezen. |
| SecurityException | De aanroeper heeft niet de vereiste toestemming om de *fileInfo* te openen. |
| ArgumentException | Het bestandspad is leeg of bevat alleen witruimtes. |
| FileNotFoundException | Het bestand is niet gevonden. |
| UnauthorizedAccessException | Pad naar bestand is alleen-lezen of is een map. |
| ArgumentNullException | *fileInfo* is null. |
| DirectoryNotFoundException | Het opgegeven pad is ongeldig, bijvoorbeeld omdat het zich op een niet-toegewezen station bevindt. |
| IOException | Het bestand is al geopend. |
| OperationCanceledException | In .NET Framework 4.0 en hoger: Wordt gegooid wanneer de extractie wordt geannuleerd via het opgegeven annulerings‑token. |
| ObjectDisposedException | Wordt opgegooid als de bronstroom is verwijderd. |

## Opmerkingen

Doet niets voor mapitem.

## Voorbeelden

```csharp
using (var lhaFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LhaArchive(lhaFile))
    {
        archive.Entries[0].Extract(new FileInfo("extracted.bin"));
    }
}
```

### Zie ook

* class [LhaArchiveEntry](../)
* namespace [Aspose.Zip.Lha](../../lhaarchiveentry/)
* assembly [Aspose.Zip](../../../)


