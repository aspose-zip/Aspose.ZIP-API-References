---
title: WimFileEntry.Extract
second_title: Aspose.ZIP voor .NET API-referentie
description: WimFileEntry methode. Extraheert de invoer naar het bestandssysteem via het opgegeven pad.
type: docs
weight: 20
url: /nl/net/aspose.zip.wim/wimfileentry/extract/
---
## Extract(string) {#extract}

Extraheert de invoer naar het bestandssysteem via het opgegeven pad.

```csharp
public FileInfo Extract(string path)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | String | Het pad naar het doelbestand. Als het bestand al bestaat, wordt het overschreven. |

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
using (var archive = new WimArchive("archive.wim"))
{
    archive.Images[0].RootDirectory.Files[0].Extract("data.bin");
}
```

### Zie ook

* class [WimFileEntry](../)
* naamruimte [Aspose.Zip.Wim](../../wimfileentry/)
* montage [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

Extraheert de ingang van de geleverde stream.

```csharp
public void Extract(Stream destination)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| destination | Stream | Bestemmingsstroom. Moet beschrijfbaar zijn. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentException | *destination* ondersteunt schrijven niet. |

### Voorbeelden

Pak een item uit het wi-archief uit.

```csharp
using (var archive = new WimArchive("archive.wim"))
{
    archive.Images[0].RootDirectory.Files[0].Extract(httpResponseStream);
}
```

### Zie ook

* class [WimFileEntry](../)
* naamruimte [Aspose.Zip.Wim](../../wimfileentry/)
* montage [Aspose.Zip](../../../)


