---
title: Class ParallelOptions
second_title: Aspose.ZIP voor .NET API-referentie
description: Aspose.Zip.Saving.ParallelOptions klas. Opties voor parallelle compressie.
type: docs
weight: 490
url: /nl/net/aspose.zip.saving/paralleloptions/
---
## ParallelOptions class

Opties voor parallelle compressie.

```csharp
public class ParallelOptions
```

## Constructeurs

| Naam | Beschrijving |
| --- | --- |
| [ParallelOptions](paralleloptions/)() | De standaard constructeur. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [AvailableMemorySize](../../aspose.zip.saving/paralleloptions/availablememorysize/) { get; set; } | Haalt of stelt geheugenschatting in megabytes beschikbaar om gecomprimeerde ingangen te huisvesten zonder naar schijf te wisselen. Deze waarde is alleen zinvol als[`ParallelCompressInMemory`](./parallelcompressinmemory/) instelling is binnenAuto modus. |
| [ParallelCompressInMemory](../../aspose.zip.saving/paralleloptions/parallelcompressinmemory/) { get; set; } | Haalt of stelt een waarde in die aangeeft hoe parallelle benadering moet worden gebruikt. |

### Opmerkingen

Deze opties beheren gelijktijdige compressie door meerdere CPU-kernen.

### Voorbeelden

```csharp
using (var archive = new Archive())
{
    archive.CreateEntries("DirToCompress");
    archive.Save("archive.zip", new ArchiveSaveOptions() { ParallelOptions = new ParallelOptions { ParallelCompressInMemory = mode, AvailableMemorySize = 4000 } });
}
```

### Zie ook

* naamruimte [Aspose.Zip.Saving](../../aspose.zip.saving/)
* montage [Aspose.Zip](../../)


