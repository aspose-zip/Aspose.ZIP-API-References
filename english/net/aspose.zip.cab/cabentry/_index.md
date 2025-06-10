---
title: Class CabEntry
second_title: Aspose.ZIP for .NET API Reference
description: Aspose.Zip.Cab.CabEntry class. Represents a single file within cab archive
type: docs
weight: 170
url: /net/aspose.zip.cab/cabentry/
---
## CabEntry class

Represents a single file within cab archive.

```csharp
public sealed class CabEntry : IArchiveFileEntry
```

## Properties

| Name | Description |
| --- | --- |
| [Length](../../aspose.zip.cab/cabentry/length/) { get; } | Gets the length of the entry in bytes. |
| [ModificationTime](../../aspose.zip.cab/cabentry/modificationtime/) { get; } | Gets last modified date and time. |
| [Name](../../aspose.zip.cab/cabentry/name/) { get; } | Gets name of the entry within the archive. |

## Methods

| Name | Description |
| --- | --- |
| [Extract](../../aspose.zip.cab/cabentry/extract/#extract_1)(Stream) | Extracts the entry to the stream provided. |
| [Extract](../../aspose.zip.cab/cabentry/extract/#extract)(string) | Extracts the entry to the filesystem by the path provided. |
| [Open](../../aspose.zip.cab/cabentry/open/)() | Opens the entry for extraction and provides a stream with entry content. |
| override [ToString](../../aspose.zip.cab/cabentry/tostring/)() |  |

### See Also

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Cab](../../aspose.zip.cab/)
* assembly [Aspose.Zip](../../)


