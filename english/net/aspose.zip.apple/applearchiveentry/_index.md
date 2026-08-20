---
title: Class AppleArchiveEntry
second_title: Aspose.ZIP for .NET API Reference
description: Aspose.Zip.Apple.AppleArchiveEntry class. Represents a file or directory entry within an AppleArchive
type: docs
weight: 70
url: /net/aspose.zip.apple/applearchiveentry/
---
## AppleArchiveEntry class

Represents a file or directory entry within an [`AppleArchive`](../applearchive/).

```csharp
public sealed class AppleArchiveEntry : IArchiveFileEntry
```

## Properties

| Name | Description |
| --- | --- |
| [IsDirectory](../../aspose.zip.apple/applearchiveentry/isdirectory/) { get; } | Gets a value indicating whether the entry represents a directory. |
| [Length](../../aspose.zip.apple/applearchiveentry/length/) { get; } | Gets the uncompressed length of the entry in bytes. |
| [Name](../../aspose.zip.apple/applearchiveentry/name/) { get; } | Gets the path of the entry inside the archive. |

## Methods

| Name | Description |
| --- | --- |
| [Extract](../../aspose.zip.apple/applearchiveentry/extract/#extract_1)(Stream) | Extracts the entry to the stream provided. |
| [Extract](../../aspose.zip.apple/applearchiveentry/extract/#extract)(string) | Extracts the entry to the filesystem by the path provided. |
| [Open](../../aspose.zip.apple/applearchiveentry/open/)() | Opens the entry for extraction and provides a stream with the entry content. |

## Remarks

An instance of this class can represent either an entry parsed from an existing Apple Archive or an entry added to an archive being composed.

### See Also

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Apple](../../aspose.zip.apple/)
* assembly [Aspose.Zip](../../)


