---
title: SnappyArchive.Save
second_title: Aspose.ZIP voor .NET API-referentie
description: SnappyArchive methode. Slaat pittig archief op in de geleverde stream.
type: docs
weight: 40
url: /nl/net/aspose.zip.snappy/snappyarchive/save/
---
## Save(Stream) {#save_1}

Slaat pittig archief op in de geleverde stream.

```csharp
public void Save(Stream output)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| output | Stream | Bestemmingsstroom. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentException | *output* ondersteunt het zoeken niet. |
| ArgumentNullException | *output* is niets. |

### Opmerkingen

*output* moet vindbaar zijn.

### Voorbeelden

```csharp
using (FileStream snappyFile = File.Open("archive.snappy", FileMode.Create))
{
    using (var archive = new SnappyArchive())
    {
        archive.SetSource("data.bin");
        archive.Save(snappyFile);
     }
}
```

### Zie ook

* class [SnappyArchive](../)
* naamruimte [Aspose.Zip.Snappy](../../snappyarchive/)
* montage [Aspose.Zip](../../../)

---

## Save(FileInfo) {#save}

Slaat pittig archief op in opgegeven bestemmingsbestand.

```csharp
public void Save(FileInfo destination)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| destination | FileInfo | FileInfo die wordt geopend als bestemmingsstroom. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| SecurityException | De beller heeft niet de vereiste toestemming om het*destination*. |
| ArgumentException | Bestandspad is leeg of bevat alleen spaties. |
| FileNotFoundException | Het bestand is niet gevonden. |
| UnauthorizedAccessException | Pad naar bestand is alleen-lezen of is een directory. |
| ArgumentNullException | *destination* is niets. |
| DirectoryNotFoundException | Het opgegeven pad is ongeldig, omdat het zich bijvoorbeeld op een niet-toegewezen schijf bevindt. |
| IOException | Het bestand is al geopend. |

### Voorbeelden

```csharp
using (var archive = new SnappyArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(new FileInfo("archive.snappy"));
}
```

### Zie ook

* class [SnappyArchive](../)
* naamruimte [Aspose.Zip.Snappy](../../snappyarchive/)
* montage [Aspose.Zip](../../../)

---

## Save(string) {#save_2}

Slaat pittig archief op in opgegeven bestemmingsbestand.

```csharp
public void Save(string destinationFileName)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| destinationFileName | String | Het pad van het aan te maken archief. Als de opgegeven bestandsnaam naar een bestaand bestand verwijst, wordt dit overschreven. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentNullException | *destinationFileName* is niets. |
| SecurityException | De beller heeft niet de vereiste toegangsrechten. |
| ArgumentException | De*destinationFileName* is leeg, bevat alleen spaties of bevat ongeldige tekens. |
| UnauthorizedAccessException | Toegang tot dossier*destinationFileName* wordt ontkend. |
| PathTooLongException | De opgegeven*destinationFileName*, bestandsnaam of beide overschrijden de door het systeem gedefinieerde maximale lengte. Op Windows-gebaseerde platforms moeten paden bijvoorbeeld uit minder dan 248 tekens bestaan en moeten bestandsnamen uit minder dan 260 tekens bestaan. |
| NotSupportedException | Dossier bij*destinationFileName* bevat een dubbele punt (:) in het midden van de tekenreeks. |

### Voorbeelden

```csharp
using (var archive = new SnappyArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("result.snappy");
}
```

### Zie ook

* class [SnappyArchive](../)
* naamruimte [Aspose.Zip.Snappy](../../snappyarchive/)
* montage [Aspose.Zip](../../../)


