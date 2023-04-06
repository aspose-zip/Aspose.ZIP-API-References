---
title: Bzip2Archive.Save
second_title: Aspose.ZIP voor .NET API-referentie
description: Bzip2Archive methode. Slaat archief op in de geleverde stream.
type: docs
weight: 50
url: /nl/net/aspose.zip.bzip2/bzip2archive/save/
---
## Save(Stream, Bzip2SaveOptions) {#save}

Slaat archief op in de geleverde stream.

```csharp
public void Save(Stream outputStream, Bzip2SaveOptions saveOptions = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| outputStream | Stream | Bestemmingsstroom. |
| saveOptions | Bzip2SaveOptions | Opties voor het opslaan van een bzip2-archief. Indien niet gespecificeerd, zou een blokgrootte van 900 Kb worden gebruikt. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| InvalidOperationException | De bron van de te archiveren gegevens is niet opgegeven. |
| ArgumentException | *outputStream* is niet beschrijfbaar. |
| UnauthorizedAccessException | Bestandsbron is alleen-lezen of is een map. |
| DirectoryNotFoundException | Het opgegeven bestandsbronpad is ongeldig, omdat het zich bijvoorbeeld op een niet-toegewezen schijf bevindt. |
| IOException | De bestandsbron is al geopend. |

### Opmerkingen

*outputStream*moet beschrijfbaar zijn.

### Voorbeelden

Schrijft gecomprimeerde gegevens naar http-antwoordstroom.

```csharp
using (var archive = new Bzip2Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(httpResponse.OutputStream);
}
```

### Zie ook

* class [Bzip2SaveOptions](../../bzip2saveoptions/)
* class [Bzip2Archive](../)
* naamruimte [Aspose.Zip.Bzip2](../../bzip2archive/)
* montage [Aspose.Zip](../../../)

---

## Save(string, Bzip2SaveOptions) {#save_1}

Slaat archief op in opgegeven bestemmingsbestand.

```csharp
public void Save(string destinationFileName, Bzip2SaveOptions saveOptions = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| destinationFileName | String | Het pad van het aan te maken archief. Als de opgegeven bestandsnaam naar een bestaand bestand verwijst, wordt dit overschreven. |
| saveOptions | Bzip2SaveOptions | Opties voor het opslaan van een bzip2-archief. Indien niet gespecificeerd, zou een blokgrootte van 900 Kb worden gebruikt. |

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

Schrijft gecomprimeerde gegevens naar bestand.

```csharp
using (var archive = new Bzip2Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("data.bz2");
}
```

### Zie ook

* class [Bzip2SaveOptions](../../bzip2saveoptions/)
* class [Bzip2Archive](../)
* naamruimte [Aspose.Zip.Bzip2](../../bzip2archive/)
* montage [Aspose.Zip](../../../)


