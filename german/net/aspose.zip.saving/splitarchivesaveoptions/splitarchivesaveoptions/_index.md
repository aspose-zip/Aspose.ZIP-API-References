---
title: SplitArchiveSaveOptions.SplitArchiveSaveOptions
second_title: Aspose.ZIP für .NET-API-Referenz
description: SplitArchiveSaveOptions constructeur. Instanziiert Einstellungen zum Speichern eines ZIPArchivs mit mehreren Volumes.
type: docs
weight: 10
url: /de/net/aspose.zip.saving/splitarchivesaveoptions/splitarchivesaveoptions/
---
## SplitArchiveSaveOptions constructor

Instanziiert Einstellungen zum Speichern eines ZIP-Archivs mit mehreren Volumes.

```csharp
public SplitArchiveSaveOptions(string fileName, uint segmentSize)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | String | Name für Volumes. Kann mit oder ohne .zip-Erweiterung sein. |
| segmentSize | UInt32 | Größe des Volumens. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentOutOfRangeException | Die Segmentgröße beträgt weniger als 65536 Byte. |

### Bemerkungen

Einige Volumina können kleiner sein als*segmentSize*. In den meisten Fällen wird das letzte Segment weniger sein, aber in seltenen Fällen können dies auch die regulären Segmente sein.

Die Dateinamen lauten wie folgt:*fileName* .z01,*fileName* .z02, ...,*fileName* .z(n-1),*fileName*.Reißverschluss.

### Siehe auch

* class [SplitArchiveSaveOptions](../)
* namensraum [Aspose.Zip.Saving](../../splitarchivesaveoptions/)
* Montage [Aspose.Zip](../../../)


