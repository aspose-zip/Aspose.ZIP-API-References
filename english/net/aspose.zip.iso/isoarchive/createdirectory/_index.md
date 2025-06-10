---
title: IsoArchive.CreateDirectory
second_title: Aspose.ZIP for .NET API Reference
description: IsoArchive method. Adds a directory to the ISO image
type: docs
weight: 30
url: /net/aspose.zip.iso/isoarchive/createdirectory/
---
## IsoArchive.CreateDirectory method

Adds a directory to the ISO image.

```csharp
public IsoEntry CreateDirectory(string name)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | Path of the directory in the ISO. |

### Return Value

The ISO entry composed.

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | The archive is opened for extraction. |
| ArgumentNullException | `name` is null or empty. |
| ObjectDisposedException | Archive has been disposed and cannot be used. |

### See Also

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


