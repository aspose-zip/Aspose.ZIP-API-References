---
title: SplitSevenZipArchiveSaveOptions.SplitSevenZipArchiveSaveOptions
second_title: Aspose.ZIP für .NET-API-Referenz
description: SplitSevenZipArchiveSaveOptions constructeur. Instanziiert Einstellungen zum Speichern eines 7zArchivs mit mehreren Volumes.
type: docs
weight: 10
url: /de/net/aspose.zip.saving/splitsevenziparchivesaveoptions/splitsevenziparchivesaveoptions/
---
## SplitSevenZipArchiveSaveOptions constructor

Instanziiert Einstellungen zum Speichern eines 7z-Archivs mit mehreren Volumes.

```csharp
public SplitSevenZipArchiveSaveOptions(string fileName, uint segmentSize)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | String | Name für Volumes. Kann mit oder ohne .7z-Erweiterung sein. |
| segmentSize | UInt32 | Größe des Volumens. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentOutOfRangeException | *segmentSize* ist kleiner als 100. |

### Bemerkungen

Einige Volumina können kleiner sein als*segmentSize*. In den meisten Fällen wird das letzte Segment weniger sein, aber in seltenen Fällen können dies auch die regulären Segmente sein.

Die Dateinamen lauten wie folgt:*fileName* .7z.001,*fileName* .7z.002, ...,*fileName*.7z.(n).

### Siehe auch

* class [SplitSevenZipArchiveSaveOptions](../)
* namensraum [Aspose.Zip.Saving](../../splitsevenziparchivesaveoptions/)
* Montage [Aspose.Zip](../../../)


