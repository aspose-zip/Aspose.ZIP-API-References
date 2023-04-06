---
title: SevenZipArchive.SaveSplit
second_title: Aspose.ZIP voor .NET API-referentie
description: SevenZipArchive methode. Slaat archief met meerdere volumes op in de opgegeven doelmap.
type: docs
weight: 90
url: /nl/net/aspose.zip.sevenzip/sevenziparchive/savesplit/
---
## SevenZipArchive.SaveSplit method

Slaat archief met meerdere volumes op in de opgegeven doelmap.

```csharp
public void SaveSplit(string destinationDirectory, SplitSevenZipArchiveSaveOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| destinationDirectory | String | Het pad naar de map waar archiefsegmenten moeten worden gemaakt. |
| options | SplitSevenZipArchiveSaveOptions | Opties voor archiefopslag, inclusief bestandsnaam. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| InvalidOperationException | Dit archief is geopend vanuit een bestaande bron. |
| ArgumentNullException | *destinationDirectory* is niets. |
| SecurityException | De beller heeft niet de vereiste toestemming om toegang te krijgen tot het telefoonboek. |
| ArgumentException | *destinationDirectory* bevat ongeldige tekens zoals ", &gt;, &lt; of &#x7C;. |
| PathTooLongException | Het opgegeven pad overschrijdt de door het systeem gedefinieerde maximale lengte. |

### Opmerkingen

Deze methode bestaat uit verschillende (`N`) bestanden bestandsnaam.7z.001, bestandsnaam.7z.002, ..., bestandsnaam.7z.(n).

Kan bestaand archief niet multi-volume maken.

### Voorbeelden

```csharp
using (SevenZipArchive archive = new SevenZipArchive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.SaveSplit(@"C:\Folder",  new SplitSevenZipArchiveSaveOptions("volume", 65536));
}
```

### Zie ook

* class [SplitSevenZipArchiveSaveOptions](../../../aspose.zip.saving/splitsevenziparchivesaveoptions/)
* class [SevenZipArchive](../)
* naamruimte [Aspose.Zip.SevenZip](../../sevenziparchive/)
* montage [Aspose.Zip](../../../)


