---
title: ArchiveInstanceInfo.GetArchiveFormatInfo
second_title: Aspose.ZIP voor .NET API-referentie
description: ArchiveInstanceInfo methode. Krijgt informatie over archiefformaat.
type: docs
weight: 50
url: /nl/net/aspose.zip.archiveinfo/archiveinstanceinfo/getarchiveformatinfo/
---
## GetArchiveFormatInfo(string) {#getarchiveformatinfo_1}

Krijgt informatie over archiefformaat.

```csharp
public static ArchiveFormatInfo GetArchiveFormatInfo(string fileName)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fileName | String | De bestandsnaam van het archiefbestand. |

### Winstwaarde

Informatie over archiefindeling of null als indeling niet is gedetecteerd.

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

* class [ArchiveFormatInfo](../../archiveformatinfo/)
* class [ArchiveInstanceInfo](../)
* naamruimte [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* montage [Aspose.Zip](../../../)

---

## GetArchiveFormatInfo(Stream) {#getarchiveformatinfo}

Krijgt informatie over archiefformaat.

```csharp
public static ArchiveFormatInfo GetArchiveFormatInfo(Stream stream)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stream | Stream | De stroom van het archiefbestand. |

### Winstwaarde

Informatie over archiefindeling of null als indeling niet is gedetecteerd.

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentNullException | *stream* is niets. |
| ArgumentException | *stream* is niet zoek. |

### Zie ook

* class [ArchiveFormatInfo](../../archiveformatinfo/)
* class [ArchiveInstanceInfo](../)
* naamruimte [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* montage [Aspose.Zip](../../../)


