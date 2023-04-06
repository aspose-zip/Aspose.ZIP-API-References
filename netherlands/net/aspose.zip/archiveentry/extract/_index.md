---
title: ArchiveEntry.Extract
second_title: Aspose.ZIP voor .NET API-referentie
description: ArchiveEntry methode. Extraheert de invoer naar het bestandssysteem via het opgegeven pad.
type: docs
weight: 100
url: /nl/net/aspose.zip/archiveentry/extract/
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
| InvalidDataException | CRC- of MAC-verificatie mislukt voor het item. |

### Voorbeelden

Pak twee ingangen van het zip-archief uit, elk met een eigen wachtwoord

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Open))
{
    using (Archive archive = new Archive(zipFile))
    {
        archive.Entries[0].Extract("first.bin", "first_pass");
        archive.Entries[1].Extract("second.bin", "second_pass");
    }
}
```

### Zie ook

* class [ArchiveEntry](../)
* naamruimte [Aspose.Zip](../../archiveentry/)
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
| InvalidDataException | CRC- of MAC-verificatie mislukt voor het item. |
| ArgumentException | *destination* ondersteunt schrijven niet. |

### Voorbeelden

Pak een item uit het zip-archief uit met een wachtwoord.

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Open))
{
    using (Archive archive = new Archive(zipFile))
    {
        archive.Entries[0].Extract(httpResponseStream, "p@s$");
    }
}
```

### Zie ook

* class [ArchiveEntry](../)
* naamruimte [Aspose.Zip](../../archiveentry/)
* montage [Aspose.Zip](../../../)


