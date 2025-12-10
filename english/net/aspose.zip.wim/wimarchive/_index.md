---
title: Class WimArchive
second_title: Aspose.ZIP for .NET API Reference
description: Aspose.Zip.Wim.WimArchive class. This class represents a wim archive file
type: docs
weight: 1100
url: /net/aspose.zip.wim/wimarchive/
---
## WimArchive class

This class represents a wim archive file.

```csharp
public class WimArchive : IArchive
```

## Constructors

| Name | Description |
| --- | --- |
| [WimArchive](wimarchive/#constructor)(Stream, WimLoadOptions) | Initializes a new instance of the `WimArchive` class and composes an entry list can be extracted from the archive. |
| [WimArchive](wimarchive/#constructor_1)(string, WimLoadOptions) | Initializes a new instance of the `WimArchive` class and composes an entry list can be extracted from the archive. |

## Properties

| Name | Description |
| --- | --- |
| [BootImageIndex](../../aspose.zip.wim/wimarchive/bootimageindex/) { get; } | Gets the (zero-based) index of the bootable image. |
| [FileFormatVersion](../../aspose.zip.wim/wimarchive/fileformatversion/) { get; } | Gets the version of the file format. |
| [Guid](../../aspose.zip.wim/wimarchive/guid/) { get; } | Gets the identifying GUID for the archive. |
| [Images](../../aspose.zip.wim/wimarchive/images/) { get; } | Gets entries of [`WimImage`](../wimimage/) type constituting the archive. |
| [Manifest](../../aspose.zip.wim/wimarchive/manifest/) { get; } | Gets the embedded manifest describing the file and the contained images. |

## Methods

| Name | Description |
| --- | --- |
| [Dispose](../../aspose.zip.wim/wimarchive/dispose/)() | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [ExtractToDirectory](../../aspose.zip.wim/wimarchive/extracttodirectory/)(string) | Extracts the archive to the file by path. |

### See Also

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Wim](../../aspose.zip.wim/)
* assembly [Aspose.Zip](../../)


