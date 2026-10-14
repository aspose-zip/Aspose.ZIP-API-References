---
title: "WimArchive.ExtractToDirectory"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "WimArchive-methode. Extraheert het archief naar het bestand op het opgegeven pad"
type: docs
weight: 90
url: /nl/net/aspose.zip.wim/wimarchive/extracttodirectory/
---
## WimArchive.ExtractToDirectory method

Extraheert het archief naar het bestand via pad.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| destinationDirectory | String | Het pad naar de map waarin de uitgepakte bestanden moeten worden geplaatst. |

### Retourwaarde

Info van het geëxtraheerde bestand.

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ObjectDisposedException | Archief is verwijderd en kan niet worden gebruikt. |
| ArgumentNullException | *destinationDirectory* is null |
| PathTooLongException | Het opgegeven pad, bestandsnaam, of beide overschrijden de door het systeem gedefinieerde maximale lengte. Bijvoorbeeld, op Windows-platformen moeten paden korter zijn dan 248 tekens en bestandsnamen korter dan 260 tekens. |
| SecurityException | De aanroeper heeft niet de vereiste toestemming om toegang te krijgen tot de bestaande map. |
| NotSupportedException | Als de map niet bestaat, bevat het pad een dubbelepunt (:) dat geen onderdeel is van een stationslabel (\"C:\\") - of - WIM‑archief is multipart. |
| ArgumentException | pad is een tekenreeks met lengte nul, bevat alleen witruimte, of bevat één of meer ongeldige tekens. Je kunt ongeldige tekens opvragen met de methode System.IO.Path.GetInvalidPathChars. -of- pad begint met, of bevat, alleen een dubbelepunt (:). |
| IOException | De map opgegeven door pad is een bestand. -or- De netwerknaam is niet bekend. |
| InvalidDataException | Het archief is beschadigd. |
| OperationCanceledException | In .NET Framework 4.0 en hoger: Wordt gegooid wanneer de extractie wordt geannuleerd via het opgegeven annulerings‑token. |

### Zie ook

* class [WimArchive](../)
* namespace [Aspose.Zip.Wim](../../wimarchive/)
* assembly [Aspose.Zip](../../../)


