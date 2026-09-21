---
title: IVolumeStreamProvider.VolumeCompleted
second_title: Aspose.ZIP for .NET API Reference
description: IVolumeStreamProvider method. Called after a volume of a split multivolume archive has been written
type: docs
weight: 20
url: /net/aspose.zip.saving/ivolumestreamprovider/volumecompleted/
---
## IVolumeStreamProvider.VolumeCompleted method

Called after a volume of a split (multivolume) archive has been written.

```csharp
public void VolumeCompleted(int index, Stream s, bool isLast)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The number of volume written, starting from zero. |
| s | Stream | The destination stream the volume written to. |
| isLast | Boolean | Whether the volume finishes the archive. |

### See Also

* interface [IVolumeStreamProvider](../)
* namespace [Aspose.Zip.Saving](../../ivolumestreamprovider/)
* assembly [Aspose.Zip](../../../)


