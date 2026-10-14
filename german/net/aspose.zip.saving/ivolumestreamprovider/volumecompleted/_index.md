---
title: "IVolumeStreamProvider.VolumeCompleted"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "IVolumeStreamProvider‑Methode. Wird aufgerufen, nachdem ein Volume eines geteilten Mehrvolumen‑Archivs geschrieben wurde"
type: docs
weight: 20
url: /de/net/aspose.zip.saving/ivolumestreamprovider/volumecompleted/
---
## IVolumeStreamProvider.VolumeCompleted method

Wird aufgerufen, nachdem ein Volume eines geteilten (mehrteiligen) Archivs geschrieben wurde.

```csharp
public void VolumeCompleted(int index, Stream s, bool isLast)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| index | Int32 | Die Anzahl der geschriebenen Volumes, beginnend bei Null. |
| s | Stream | Der Ziel‑Stream, in den das Volume geschrieben wurde. |
| isLast | Boolean | Ob das Volume das Archiv abschließt. |

### Siehe auch

* interface [IVolumeStreamProvider](../)
* namespace [Aspose.Zip.Saving](../../ivolumestreamprovider/)
* assembly [Aspose.Zip](../../../)


