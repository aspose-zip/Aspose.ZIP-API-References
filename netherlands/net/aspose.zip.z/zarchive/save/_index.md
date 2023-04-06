---
title: ZArchive.Save
second_title: Aspose.ZIP voor .NET API-referentie
description: ZArchive methode. Slaat xzarchief op in de geleverde stream.
type: docs
weight: 40
url: /nl/net/aspose.zip.z/zarchive/save/
---
## Save(Stream) {#save}

Slaat xz-archief op in de geleverde stream.

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
using (FileStream zFile = File.Open("data.bin.z", FileMode.Create))
{
    using (var archive = new ZArchive())
    {
        archive.SetSource("data.bin");
        archive.Save(zFile);
     }
}
```

### Zie ook

* class [ZArchive](../)
* naamruimte [Aspose.Zip.Z](../../zarchive/)
* montage [Aspose.Zip](../../../)

---

## Save(string) {#save_1}

Slaat Z-archief op in opgegeven bestemmingsbestand.

```csharp
public void Save(string destinationFileName)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| destinationFileName | String | +Het pad van het aan te maken archief. Als de opgegeven bestandsnaam naar een bestaand bestand verwijst, wordt dit overschreven. |

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
using (var archive = new ZArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("data.bin.Z");
}
```

### Zie ook

* class [ZArchive](../)
* naamruimte [Aspose.Zip.Z](../../zarchive/)
* montage [Aspose.Zip](../../../)


