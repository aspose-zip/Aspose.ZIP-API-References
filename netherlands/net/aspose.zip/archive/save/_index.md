---
title: Archive.Save
second_title: Aspose.ZIP voor .NET API-referentie
description: Archive methode. Slaat archief op in de geleverde stream.
type: docs
weight: 90
url: /nl/net/aspose.zip/archive/save/
---
## Save(Stream, ArchiveSaveOptions) {#save}

Slaat archief op in de geleverde stream.

```csharp
public void Save(Stream outputStream, ArchiveSaveOptions saveOptions = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| outputStream | Stream | Bestemmingsstroom. |
| saveOptions | ArchiveSaveOptions | Opties voor archiefopslag. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentException | *outputStream* is niet beschrijfbaar. |

### Opmerkingen

*outputStream*moet beschrijfbaar zijn.

### Voorbeelden

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry.bin", "data.bin");
        archive.Save(zipFile);
    }
}
```

### Zie ook

* class [ArchiveSaveOptions](../../../aspose.zip.saving/archivesaveoptions/)
* class [Archive](../)
* naamruimte [Aspose.Zip](../../archive/)
* montage [Aspose.Zip](../../../)

---

## Save(string, ArchiveSaveOptions) {#save_1}

Slaat archief op in opgegeven bestemmingsbestand.

```csharp
public void Save(string destinationFileName, ArchiveSaveOptions saveOptions = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| destinationFileName | String | Het pad van het aan te maken archief. Als de opgegeven bestandsnaam naar een bestaand bestand verwijst, wordt dit overschreven. |
| saveOptions | ArchiveSaveOptions | Opties voor archiefopslag. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentNullException | *destinationFileName* is niets. |
| SecurityException | De beller heeft niet de vereiste toegangsrechten. |
| ArgumentException | De*destinationFileName* is leeg, bevat alleen spaties of bevat ongeldige tekens. |
| UnauthorizedAccessException | Toegang tot dossier*destinationFileName* wordt ontkend. |
| PathTooLongException | De opgegeven*destinationFileName*, bestandsnaam of beide overschrijden de door het systeem gedefinieerde maximale lengte. Op Windows-gebaseerde platforms moeten paden bijvoorbeeld uit minder dan 248 tekens bestaan en moeten bestandsnamen uit minder dan 260 tekens bestaan. |
| NotSupportedException | Dossier bij*destinationFileName* bevat een dubbele punt (:) in het midden van de tekenreeks. |

### Opmerkingen

Het is mogelijk om een archief op te slaan in hetzelfde pad als waaruit het is geladen. Dit wordt echter niet aanbevolen, omdat deze aanpak gebruikmaakt van kopiëren naar een tijdelijk bestand.

### Voorbeelden

```csharp
using (var archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.Save("archive.zip",  new ArchiveSaveOptions() { Encoding = Encoding.ASCII });
}
```

### Zie ook

* class [ArchiveSaveOptions](../../../aspose.zip.saving/archivesaveoptions/)
* class [Archive](../)
* naamruimte [Aspose.Zip](../../archive/)
* montage [Aspose.Zip](../../../)


