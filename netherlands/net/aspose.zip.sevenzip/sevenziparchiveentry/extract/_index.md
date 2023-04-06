---
title: SevenZipArchiveEntry.Extract
second_title: Aspose.ZIP voor .NET API-referentie
description: SevenZipArchiveEntry methode. Extraheert de invoer naar het bestandssysteem via het opgegeven pad.
type: docs
weight: 80
url: /nl/net/aspose.zip.sevenzip/sevenziparchiveentry/extract/
---
## Extract(string, string) {#extract}

Extraheert de invoer naar het bestandssysteem via het opgegeven pad.

```csharp
public FileInfo Extract(string path, string password = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | String | Het pad naar het doelbestand. Als het bestand al bestaat, wordt het overschreven. |
| password | String | Optioneel wachtwoord voor decodering. |

### Winstwaarde

De bestandsinfo van het samengestelde bestand.

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentNullException | *path* is niets. |
| SecurityException | De beller heeft niet de vereiste toegangsrechten. |
| ArgumentException | De*path* is leeg, bevat alleen spaties of bevat ongeldige tekens. |
| UnauthorizedAccessException | Toegang tot dossier*path* wordt ontkend. |
| PathTooLongException | De opgegeven*path*, bestandsnaam of beide overschrijden de door het systeem gedefinieerde maximale lengte. Op Windows-gebaseerde platforms moeten paden bijvoorbeeld uit minder dan 248 tekens bestaan en moeten bestandsnamen uit minder dan 260 tekens bestaan. |
| NotSupportedException | Dossier bij*path* bevat een dubbele punt (:) in het midden van de tekenreeks. |

### Voorbeelden

```csharp
using (var archive = new SevenZipArchive("archive.7z"))
{
    archive.Entries[0].Extract("data.bin");
}
```

### Zie ook

* class [SevenZipArchiveEntry](../)
* naamruimte [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* montage [Aspose.Zip](../../../)

---

## Extract(Stream, string) {#extract_1}

Extraheert de ingang van de geleverde stream.

```csharp
public void Extract(Stream destination, string password = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| destination | Stream | Bestemmingsstroom. Moet beschrijfbaar zijn. |
| password | String | Optioneel wachtwoord voor decodering. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentException | *destination* ondersteunt schrijven niet. |
| InvalidOperationException | Het archief wordt niet geopend voor extractie. - of - Dit item is een directory. |
| InvalidDataException | Verkeerde gegevens in de invoer. |

### Voorbeelden

Pak een item uit het zip-archief uit met een wachtwoord.

```csharp
using (var archive = new SevenZipArchive("archive.7z"))
{
    archive.Entries[0].Extract(httpResponseStream);
}
```

### Zie ook

* class [SevenZipArchiveEntry](../)
* naamruimte [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* montage [Aspose.Zip](../../../)


