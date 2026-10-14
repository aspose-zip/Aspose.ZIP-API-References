---
title: "Bzip2Archive.ExtractToDirectory"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "Bzip2Archive method. Extraheert de inhoud van het archief naar de opgegeven map."
type: docs
weight: 40
url: /nl/net/aspose.zip.bzip2/bzip2archive/extracttodirectory/
---
## Bzip2Archive.ExtractToDirectory method

Extraheert de inhoud van het archief naar de opgegeven map.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| destinationDirectory | String | Het pad naar de map waarin de uitgepakte bestanden moeten worden geplaatst. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ArgumentNullException | *destinationDirectory* is null. |
| PathTooLongException | Het opgegeven pad, bestandsnaam, of beide overschrijden de door het systeem gedefinieerde maximale lengte. Bijvoorbeeld, op Windows-platformen moeten paden korter zijn dan 248 tekens en bestandsnamen korter dan 260 tekens. |
| SecurityException | De aanroeper heeft niet de vereiste toestemming om toegang te krijgen tot de bestaande map. |
| NotSupportedException | Als de map niet bestaat, bevat het pad een dubbele punt (:) die geen onderdeel is van een stationslabel ("C:\\"). |
| ArgumentException | *destinationDirectory* is een tekenreeks met lengte nul, bevat alleen witruimte, of bevat een of meer ongeldige tekens. U kunt ongeldige tekens opvragen met behulp van de methode System.IO.Path.GetInvalidPathChars. -or- pad is voorafgegaan door, of bevat, alleen een dubbelepunt (:). |
| IOException | De map opgegeven door pad is een bestand. -or- De netwerknaam is niet bekend. |
| OperationCanceledException | In .NET Framework 4.0 en hoger: Wordt gegooid wanneer de extractie wordt geannuleerd via het opgegeven annulerings‑token. |
| ObjectDisposedException | Archief is verwijderd en kan niet worden gebruikt. |

## Opmerkingen

Als de map niet bestaat, wordt deze aangemaakt.

### Zie ook

* class [Bzip2Archive](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2archive/)
* assembly [Aspose.Zip](../../../)


