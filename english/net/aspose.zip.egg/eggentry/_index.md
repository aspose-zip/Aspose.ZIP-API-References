---
title: Class EggEntry
second_title: Aspose.ZIP for .NET API Reference
description: Aspose.Zip.Egg.EggEntry class. Represents a file entry in an EGG archive with all its metadata
type: docs
weight: 470
url: /net/aspose.zip.egg/eggentry/
---
## EggEntry class

Represents a file entry in an EGG archive with all its metadata.

```csharp
public abstract class EggEntry : IArchiveFileEntry
```

## Properties

| Name | Description |
| --- | --- |
| [CompressedSize](../../aspose.zip.egg/eggentry/compressedsize/) { get; } | Gets the compressed size of the entry. |
| [IsDirectory](../../aspose.zip.egg/eggentry/isdirectory/) { get; } | Gets a value indicating whether this entry represents a directory. |
| [Length](../../aspose.zip.egg/eggentry/length/) { get; } |  |
| [ModificationTime](../../aspose.zip.egg/eggentry/modificationtime/) { get; } | Gets or sets last modified date and time. |
| [Name](../../aspose.zip.egg/eggentry/name/) { get; } | Gets the name of the entry within the archive. |
| [UncompressedSize](../../aspose.zip.egg/eggentry/uncompressedsize/) { get; } | Gets the uncompressed size of the entry. |

## Methods

| Name | Description |
| --- | --- |
| [Extract](../../aspose.zip.egg/eggentry/extract/#extract_1)(Stream) | Extracts the entry to the stream provided. |
| [Extract](../../aspose.zip.egg/eggentry/extract/#extract)(string) | Extracts the entry to the filesystem by the path provided. |
| [Open](../../aspose.zip.egg/eggentry/open/)() | Opens the entry for extraction and provides a stream with decompressed entry content. |

### See Also

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Egg](../../aspose.zip.egg/)
* assembly [Aspose.Zip](../../)


