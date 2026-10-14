---
title: "IVolumeStreamProvider.VolumeCompleted"
second_title: "Aspose.ZIP för .NET API-referens"
description: "IVolumeStreamProvider metod. Anropas efter att en volym av ett delat flervolymarkiv har skrivits"
type: docs
weight: 20
url: /sv/net/aspose.zip.saving/ivolumestreamprovider/volumecompleted/
---
## IVolumeStreamProvider.VolumeCompleted method

Kallas efter att en volym i ett delat (flervolym) arkiv har skrivits.

```csharp
public void VolumeCompleted(int index, Stream s, bool isLast)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | Int32 | Antalet volym som skrivits, med början från noll. |
| s | Ström | Destinationsströmmen som volymen skrevs till. |
| isLast | Boolean | Om volymen avslutar arkivet. |

### Se även

* interface [IVolumeStreamProvider](../)
* namespace [Aspose.Zip.Saving](../../ivolumestreamprovider/)
* assembly [Aspose.Zip](../../../)


