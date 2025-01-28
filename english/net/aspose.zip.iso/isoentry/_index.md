---
title: Class IsoEntry
second_title: Aspose.ZIP for .NET API Reference
description: Aspose.Zip.Iso.IsoEntry class. Represents an entry file or directory within an ISO archive
type: docs
weight: 310
url: /net/aspose.zip.iso/isoentry/
---
## IsoEntry class

Represents an entry (file or directory) within an ISO archive.

```csharp
public abstract class IsoEntry : IArchiveFileEntry
```

## Properties

| Name | Description |
| --- | --- |
| [IsDirectory](../../aspose.zip.iso/isoentry/isdirectory/) { get; } | Gets a value indicating whether the entry is a directory. |
| [Length](../../aspose.zip.iso/isoentry/length/) { get; } | Gets the length of the entry in bytes. |
| [Name](../../aspose.zip.iso/isoentry/name/) { get; } | Gets the name of the entry. |

## Methods

| Name | Description |
| --- | --- |
| [Extract](../../aspose.zip.iso/isoentry/extract/#extract_1)(Stream) | Extracts the entry to the stream provided. |
| [Extract](../../aspose.zip.iso/isoentry/extract/#extract)(string) | Extracts the entry to the filesystem by the path provided. |
| override [ToString](../../aspose.zip.iso/isoentry/tostring/)() | Returns a string that represents the current entry. |

### See Also

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Iso](../../aspose.zip.iso/)
* assembly [Aspose.Zip](../../)


