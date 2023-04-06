---
title: WimDirectoryEntry.ExtractToDirectory
second_title: Aspose.ZIP voor .NET API-referentie
description: WimDirectoryEntry methode. Pakt alle bestanden in de huidige map uit naar de opgegeven map.
type: docs
weight: 50
url: /nl/net/aspose.zip.wim/wimdirectoryentry/extracttodirectory/
---
## WimDirectoryEntry.ExtractToDirectory method

Pakt alle bestanden in de huidige map uit naar de opgegeven map.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| destinationDirectory | String | Het pad naar de map om de uitgepakte bestanden in te plaatsen. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentNullException | pad is nul |
| PathTooLongException | Het opgegeven pad, de bestandsnaam of beide overschrijden de door het systeem gedefinieerde maximale lengte. Op Windows-gebaseerde platforms moeten paden bijvoorbeeld uit minder dan 248 tekens bestaan en moeten bestandsnamen uit minder dan 260 tekens bestaan. |
| SecurityException | De beller heeft niet de vereiste toestemming om toegang te krijgen tot de bestaande telefoonlijst. |
| NotSupportedException | Als de directory niet bestaat, bevat het pad een dubbele punt (:) dat geen deel uitmaakt van een stationslabel ("C:\"). |
| ArgumentException | pad is een tekenreeks met lengte nul, bevat alleen witruimte of bevat een of meer ongeldige tekens. U kunt zoeken naar ongeldige tekens met behulp van de methode System.IO.Path.GetInvalidPathChars. -of- pad wordt voorafgegaan door of bevat alleen een dubbele punt (:). |
| IOException | De map gespecificeerd door pad is een bestand. -of- De netwerknaam is niet bekend. |

### Opmerkingen

Als de directory niet bestaat, wordt deze aangemaakt.

### Voorbeelden

```csharp
using (var archive = new WimArchive("archive.wim")) 
{ 
   archive.Images[0].RootDirectory.ExtractToDirectory(@"C:\\extracted");
}
```

### Zie ook

* class [WimDirectoryEntry](../)
* naamruimte [Aspose.Zip.Wim](../../wimdirectoryentry/)
* montage [Aspose.Zip](../../../)


