---
title: ArchiveInstanceInfo.GetArchiveInstanceInfo
second_title: Aspose.ZIP voor .NET API-referentie
description: ArchiveInstanceInfo methode. Haalt archiefinstantieinfo op.
type: docs
weight: 10
url: /nl/net/aspose.zip.archiveinfo/archiveinstanceinfo/getarchiveinstanceinfo/
---
## GetArchiveInstanceInfo(string) {#getarchiveinstanceinfo_1}

Haalt archiefinstantie-info op.

```csharp
public static ArchiveInstanceInfo GetArchiveInstanceInfo(string fileName)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fileName | String | De bestandsnaam van het archiefbestand. |

### Winstwaarde

Informatie over archiveringsinstantie of null als de indeling niet is gedetecteerd.

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentNullException | *fileName* is niets. |
| SecurityException | De beller heeft niet de vereiste toegangsrechten. |
| ArgumentException | De*fileName* is leeg, bevat alleen spaties of bevat ongeldige tekens. |
| UnauthorizedAccessException | Toegang tot dossier*fileName* wordt ontkend. |
| PathTooLongException | De opgegeven*fileName* de door het systeem gedefinieerde maximale lengte overschrijdt. Op Windows-gebaseerde platforms moeten paden bijvoorbeeld uit minder dan 248 tekens bestaan en moeten bestandsnamen uit minder dan 260 tekens bestaan. |
| NotSupportedException | Dossier bij*fileName* bevat een dubbele punt (:) in het midden van de tekenreeks. |
| IOException | Er is een I/O-fout opgetreden bij het openen van het bestand. |

### Zie ook

* class [ArchiveInstanceInfo](../)
* naamruimte [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* montage [Aspose.Zip](../../../)

---

## GetArchiveInstanceInfo(Stream) {#getarchiveinstanceinfo}

Haalt archiefinstantie-info op.

```csharp
public static ArchiveInstanceInfo GetArchiveInstanceInfo(Stream stream)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stream | Stream | De stroom van het archiefbestand. |

### Winstwaarde

Informatie over archiveringsinstantie of null als de indeling niet is gedetecteerd.

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentNullException | *stream* is niets. |
| ArgumentException | *stream* is niet zoek. |

### Zie ook

* class [ArchiveInstanceInfo](../)
* naamruimte [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* montage [Aspose.Zip](../../../)


