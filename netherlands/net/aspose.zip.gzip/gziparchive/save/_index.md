---
title: GzipArchive.Save
second_title: Aspose.ZIP voor .NET API-referentie
description: GzipArchive methode. Slaat archief op in de geleverde stream.
type: docs
weight: 60
url: /nl/net/aspose.zip.gzip/gziparchive/save/
---
## Save(Stream) {#save}

Slaat archief op in de geleverde stream.

```csharp
public void Save(Stream outputStream)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| outputStream | Stream | Bestemmingsstroom. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentException | *outputStream* is niet beschrijfbaar. |
| InvalidOperationException | Bron is niet opgegeven. |

### Opmerkingen

*outputStream*moet beschrijfbaar zijn.

### Voorbeelden

Schrijft gecomprimeerde gegevens naar http-antwoordstroom.

```csharp
using (var archive = new GzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(httpResponse.OutputStream);
}
```

### Zie ook

* class [GzipArchive](../)
* naamruimte [Aspose.Zip.Gzip](../../gziparchive/)
* montage [Aspose.Zip](../../../)

---

## Save(string) {#save_1}

Slaat archief op in opgegeven bestemmingsbestand.

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
using (var archive = new GzipArchive())
{
    archive.SetSource("data.bin");
    archive.Save("archive.gz");
}
```

### Zie ook

* class [GzipArchive](../)
* naamruimte [Aspose.Zip.Gzip](../../gziparchive/)
* montage [Aspose.Zip](../../../)


