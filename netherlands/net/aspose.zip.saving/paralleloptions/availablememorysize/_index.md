---
title: ParallelOptions.AvailableMemorySize
second_title: Aspose.ZIP voor .NET API-referentie
description: ParallelOptions eigendom. Haalt of stelt geheugenschatting in megabytes beschikbaar om gecomprimeerde ingangen te huisvesten zonder naar schijf te wisselen. Deze waarde is alleen zinvol alsParallelCompressInMemory instelling is binnenAuto modus.
type: docs
weight: 20
url: /nl/net/aspose.zip.saving/paralleloptions/availablememorysize/
---
## ParallelOptions.AvailableMemorySize property

Haalt of stelt geheugenschatting in megabytes beschikbaar om gecomprimeerde ingangen te huisvesten zonder naar schijf te wisselen. Deze waarde is alleen zinvol als[`ParallelCompressInMemory`](../parallelcompressinmemory/) instelling is binnenAuto modus.

```csharp
public int AvailableMemorySize { get; set; }
```

### Opmerkingen

Deze waarde wordt gebruikt om de grootste invoergrootte te berekenen die parallel met andere kan worden gecomprimeerd. Alle items boven de berekende drempel worden opeenvolgend gecomprimeerd. Het is veilig om te hebben`AvailableMemorySize` eigendom zo groot als gratis RAM en nog groter. Standaard wordt aangenomen dat u minimaal 200 MB per CPU-kern hebt.

### Zie ook

* class [ParallelOptions](../)
* naamruimte [Aspose.Zip.Saving](../../paralleloptions/)
* montage [Aspose.Zip](../../../)


