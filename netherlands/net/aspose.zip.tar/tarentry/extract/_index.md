---
title: TarEntry.Extract
second_title: Aspose.ZIP voor .NET API-referentie
description: TarEntry methode. Extraheert de invoer naar het bestandssysteem via het opgegeven pad.
type: docs
weight: 40
url: /nl/net/aspose.zip.tar/tarentry/extract/
---
## Extract(string) {#extract}

Extraheert de invoer naar het bestandssysteem via het opgegeven pad.

```csharp
public FileSystemInfo Extract(string path)
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
using (var archive = new TarArchive("archive.tar"))
{
    archive.Entries[0].Extract("data.bin");
}
```

### Zie ook

* class [TarEntry](../)
* naamruimte [Aspose.Zip.Tar](../../tarentry/)
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

Extraheer een vermelding van het tar-archief.

```csharp
using (var archive = new TarArchive("archive.tar"))
{
    archive.Entries[0].Extract(httpResponseStream);
}
```

### Zie ook

* class [TarEntry](../)
* naamruimte [Aspose.Zip.Tar](../../tarentry/)
* montage [Aspose.Zip](../../../)


