---
title: Class ArchiveEntryPlain
second_title: Aspose.ZIP for .NET API Reference
description: Aspose.Zip.ArchiveEntryPlain class. Zip entry that needs to be compressed without encryption or decompressed without decryption
type: docs
weight: 40
url: /net/aspose.zip/archiveentryplain/
---
## ArchiveEntryPlain class

Zip entry that needs to be compressed without encryption or decompressed without decryption.

```csharp
public sealed class ArchiveEntryPlain : ArchiveEntry
```

## Properties

| Name | Description |
| --- | --- |
| [Comment](../../aspose.zip/archiveentry/comment/) { get; } | Gets comment of the entry within archive. |
| [CompressedSize](../../aspose.zip/archiveentry/compressedsize/) { get; } | Gets size of compressed file. |
| [CompressionSettings](../../aspose.zip/archiveentry/compressionsettings/) { get; } | Gets settings for compression or decompression. |
| [DataSource](../../aspose.zip/archiveentry/datasource/) { get; } | Source for the entry if the entry was added to archive, not extracted. |
| [IsDirectory](../../aspose.zip/archiveentry/isdirectory/) { get; } | Gets a value indicating whether the entry represents directory. |
| [ModificationTime](../../aspose.zip/archiveentry/modificationtime/) { get; set; } | Gets or sets last modified date and time. |
| [Name](../../aspose.zip/archiveentry/name/) { get; } | Gets name of the entry within archive. |
| [UncompressedSize](../../aspose.zip/archiveentry/uncompressedsize/) { get; } | Gets size of original file. |

## Methods

| Name | Description |
| --- | --- |
| [Extract](../../aspose.zip/archiveentry/extract/)(Stream, string) | Extracts the entry to the stream provided. |
| [Extract](../../aspose.zip/archiveentry/extract/)(string, string) | Extracts the entry to the filesystem by the path provided. |
| [Open](../../aspose.zip/archiveentry/open/)(string) | Opens the entry for extraction and provides a stream with decompressed entry content. |

## Events

| Name | Description |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip/archiveentry/compressionprogressed/) | Raises when a portion of raw stream compressed. |
| event [ExtractionProgressed](../../aspose.zip/archiveentry/extractionprogressed/) | Raises when a portion of raw stream extracted. |

### See Also

* class [ArchiveEntry](../archiveentry/)
* namespace [Aspose.Zip](../../aspose.zip/)
* assembly [Aspose.Zip](../../)


