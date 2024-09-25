---
title: Class IsoArchive
second_title: Aspose.ZIP for .NET API Reference
description: Aspose.Zip.Iso.IsoArchive class. Represents an ISO archive ISO 9660
type: docs
weight: 280
url: /net/aspose.zip.iso/isoarchive/
---
## IsoArchive class

Represents an ISO archive (ISO 9660).

```csharp
public sealed class IsoArchive : IArchive
```

## Constructors

| Name | Description |
| --- | --- |
| [IsoArchive](isoarchive/#constructor)() | Initializes a new instance of the `IsoArchive` class and creates an empty ISO archive for adding new files and directories. |
| [IsoArchive](isoarchive/#constructor_1)(Stream, IsoLoadOptions) | Initializes a new instance of the `IsoArchive` class and composes entries list that can be extracted from the archive. |
| [IsoArchive](isoarchive/#constructor_2)(string, IsoLoadOptions) | Initializes a new instance of the `IsoArchive` class and composes entries list that can be extracted from the archive. |

## Properties

| Name | Description |
| --- | --- |
| [Entries](../../aspose.zip.iso/isoarchive/entries/) { get; } | Gets entries of [`IsoEntry`](../isoentry/) type constituting the archive. |
| [FileEntries](../../aspose.zip.iso/isoarchive/fileentries/) { get; } | Gets entries of [`IArchiveFileEntry`](../../aspose.zip/iarchivefileentry/) type constituting the archive. |

## Methods

| Name | Description |
| --- | --- |
| [CreateDirectory](../../aspose.zip.iso/isoarchive/createdirectory/)(string) | Adds a directory to the ISO image. |
| [CreateEntry](../../aspose.zip.iso/isoarchive/createentry/#createentry)(string) | Adds a file to the ISO image. |
| [CreateEntry](../../aspose.zip.iso/isoarchive/createentry/#createentry_1)(string, Stream) | Adds a file to the ISO image. |
| [CreateEntry](../../aspose.zip.iso/isoarchive/createentry/#createentry_2)(string, string) | Adds a file to the ISO image. |
| [Dispose](../../aspose.zip.iso/isoarchive/dispose/)() | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [ExtractToDirectory](../../aspose.zip.iso/isoarchive/extracttodirectory/)(string) | Extracts all entries to the specified directory. |
| [Save](../../aspose.zip.iso/isoarchive/save/#save)(Stream, IsoSaveOptions) | Saves the ISO image to the specified stream. |
| [Save](../../aspose.zip.iso/isoarchive/save/#save_1)(string, IsoSaveOptions) | Saves the ISO image to the specified path. |

### See Also

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Iso](../../aspose.zip.iso/)
* assembly [Aspose.Zip](../../)


