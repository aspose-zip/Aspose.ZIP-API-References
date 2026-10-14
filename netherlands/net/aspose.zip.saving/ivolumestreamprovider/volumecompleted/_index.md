---
title: "IVolumeStreamProvider.VolumeCompleted"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "IVolumeStreamProvider-methode. Wordt aangeroepen nadat een volume van een gesplitste multivolume-archief is geschreven"
type: docs
weight: 20
url: /nl/net/aspose.zip.saving/ivolumestreamprovider/volumecompleted/
---
## IVolumeStreamProvider.VolumeCompleted method

Aangeroepen nadat een volume van een gesplitst (multivolume) archief is geschreven.

```csharp
public void VolumeCompleted(int index, Stream s, bool isLast)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| index | Int32 | Het aantal geschreven volumes, beginnend bij nul. |
| s | Stream | De bestemmingsstream waaraan het volume is geschreven. |
| isLast | Boolean | Of het volume het archief voltooit. |

### Zie ook

* interface [IVolumeStreamProvider](../)
* namespace [Aspose.Zip.Saving](../../ivolumestreamprovider/)
* assembly [Aspose.Zip](../../../)


