---
title: "GetFormatInfo"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: 
type: docs
weight: 20
url: /nl/net/aspose.zip.archiveinfo/archiveformatdetector/getformatinfo/
---
## ArchiveFormatDetector.GetFormatInfo method (1 of 2)

Haalt formatinformatie op.

```csharp
public ArchiveFormatInfo GetFormatInfo(string fileName)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fileName | String | De bestandsnaam van het archiefbestand. |

### Retourwaarde

Informatie over het archiefformaat of null als het formaat niet werd gedetecteerd.

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ArgumentNullException | *fileName* is null. |
| SecurityException | De aanroeper heeft niet de vereiste toestemming om toegang te krijgen. |
| ArgumentException | De *fileName* is leeg, bevat alleen witruimtes, of bevat ongeldige tekens. |
| UnauthorizedAccessException | Toegang tot bestand *fileName* is geweigerd. |
| PathTooLongException | De opgegeven *fileName* overschrijdt de systeemgedefinieerde maximale lengte. Bijvoorbeeld, op Windows-platformen moeten paden korter zijn dan 248 tekens en bestandsnamen korter dan 260 tekens. |
| NotSupportedException | Bestand op *fileName* bevat een dubbele punt (:) in het midden van de tekenreeks. |
| IOException | Er trad een I/O-fout op tijdens het openen van het bestand. |

### Zie ook

* class [ArchiveFormatInfo](../../archiveformatinfo)
* class [ArchiveFormatDetector](../../archiveformatdetector)
* namespace [Aspose.Zip.ArchiveInfo](../../archiveformatdetector)
* assembly [Aspose.Zip](../../../)

---

## ArchiveFormatDetector.GetFormatInfo method (2 of 2)

Haalt formatinformatie op.

```csharp
public ArchiveFormatInfo GetFormatInfo(Stream stream)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stream | Stream | De stream van het archiefbestand. |

### Retourwaarde

Informatie over het archiefformaat of null als het formaat niet werd gedetecteerd.

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ArgumentNullException | *stream* is null. |
| ArgumentException | *stream* is niet doorzoekbaar. |

### Zie ook

* class [ArchiveFormatInfo](../../archiveformatinfo)
* class [ArchiveFormatDetector](../../archiveformatdetector)
* namespace [Aspose.Zip.ArchiveInfo](../../archiveformatdetector)
* assembly [Aspose.Zip](../../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor Aspose.Zip.dll -->
