---
title: Archive.SaveSplit
second_title: Aspose.ZIP voor .NET API-referentie
description: Archive methode. Slaat archief met meerdere volumes op in de opgegeven doelmap.
type: docs
weight: 100
url: /nl/net/aspose.zip/archive/savesplit/
---
## Archive.SaveSplit method

Slaat archief met meerdere volumes op in de opgegeven doelmap.

```csharp
public void SaveSplit(string destinationDirectory, SplitArchiveSaveOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| destinationDirectory | String | Het pad naar de map waar archiefsegmenten moeten worden gemaakt. |
| options | SplitArchiveSaveOptions | Opties voor archiefopslag, inclusief bestandsnaam. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| InvalidOperationException | Dit archief is geopend vanuit een bestaande bron. |
| NotSupportedException | Dit archief is zowel gecomprimeerd met de XZ-methode als versleuteld. |
| ArgumentNullException | *destinationDirectory* is niets. |
| SecurityException | De beller heeft niet de vereiste toestemming om toegang te krijgen tot het telefoonboek. |
| ArgumentException | *destinationDirectory* bevat ongeldige tekens zoals ", &gt;, &lt; of &#x7C;. |
| PathTooLongException | Het opgegeven pad overschrijdt de door het systeem gedefinieerde maximale lengte. |

### Opmerkingen

Deze methode bestaat uit verschillende (`N`) bestanden bestandsnaam.z01, bestandsnaam.z02, ..., bestandsnaam.z(n-1), bestandsnaam.zip.

Kan bestaand archief niet multi-volume maken.

### Voorbeelden

```csharp
using (Archive archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.SaveSplit(@"C:\Folder",  new SplitArchiveSaveOptions("volume", 65536));
}
```

### Zie ook

* class [SplitArchiveSaveOptions](../../../aspose.zip.saving/splitarchivesaveoptions/)
* class [Archive](../)
* naamruimte [Aspose.Zip](../../archive/)
* montage [Aspose.Zip](../../../)


