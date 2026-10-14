---
title: "LzxArchiveEntry.Extract"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "LzxArchiveEntry methode. Extraheert Lzx-archiefitem naar een bestandssysteem via pad"
type: docs
weight: 80
url: /nl/net/aspose.zip.lzx/lzxarchiveentry/extract/
---
## Extract(string) {#extract}

Extraheert Lzx-archiefvermelding naar een bestandssysteem via een pad.

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
| InvalidDataException | Controlesom komt niet overeen voor headers of data. - of - Archief is corrupt. |
| OperationCanceledException | In .NET Framework 4.0 en hoger: Wordt gegooid wanneer de extractie wordt geannuleerd via het opgegeven annulerings‑token. |
| NotSupportedException | Ongeldige compressiemethode. |
| ObjectDisposedException | Wordt opgegooid als de bronstroom is verwijderd. |
| EndOfStreamException | Wordt opgegooid wanneer het einde van de stroom onverwacht wordt bereikt. |

## Voorbeelden

```csharp
using (FileStream lzxFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LzxArchive(lhaFile))
    {
        archive.Entries[0].Extract("extracted.bin");
    }
}
```

### Zie ook

* class [LzxArchiveEntry](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchiveentry/)
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
| ArgumentException | *destination* ondersteunt geen schrijven. |
| InvalidDataException | Controlesom komt niet overeen voor headers of data. - of - Archief is corrupt. |
| ArgumentNullException | Doelstream is null. |
| NotSupportedException | Ongeldige compressiemethode. |
| OperationCanceledException | In .NET Framework 4.0 en hoger: Wordt gegooid wanneer de extractie wordt geannuleerd via het opgegeven annulerings‑token. |
| ObjectDisposedException | Wordt opgegooid als de bronstroom is verwijderd. |
| EndOfStreamException | Wordt opgegooid wanneer het einde van de stroom onverwacht wordt bereikt. |

### Zie ook

* class [LzxArchiveEntry](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchiveentry/)
* assembly [Aspose.Zip](../../../)


