---
title: Class SevenZipArchiveEntryEncrypted
second_title: Aspose.ZIP for .NET API Reference
description: Aspose.Zip.SevenZip.SevenZipArchiveEntryEncrypted class. SevenZip archive entry that needs to be compressed with encryption or decompressed with decryption
type: docs
weight: 810
url: /net/aspose.zip.sevenzip/sevenziparchiveentryencrypted/
---
## SevenZipArchiveEntryEncrypted class

SevenZip archive entry that needs to be compressed with encryption or decompressed with decryption.

```csharp
public class SevenZipArchiveEntryEncrypted : SevenZipArchiveEntry
```

## Properties

| Name | Description |
| --- | --- |
| [CompressedSize](../../aspose.zip.sevenzip/sevenziparchiveentry/compressedsize/) { get; } | Gets size of compressed file. |
| [CompressionSettings](../../aspose.zip.sevenzip/sevenziparchiveentry/compressionsettings/) { get; } | Gets settings for compression or decompression. |
| [IsDirectory](../../aspose.zip.sevenzip/sevenziparchiveentry/isdirectory/) { get; } | Gets a value indicating whether the entry represents directory. |
| [ModificationTime](../../aspose.zip.sevenzip/sevenziparchiveentry/modificationtime/) { get; } | Gets last modified date and time. |
| [Name](../../aspose.zip.sevenzip/sevenziparchiveentry/name/) { get; } | Gets name of the entry within archive. |
| [UncompressedSize](../../aspose.zip.sevenzip/sevenziparchiveentry/uncompressedsize/) { get; } | Gets size of original file. |

## Methods

| Name | Description |
| --- | --- |
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/)(Stream, string) | Extracts the entry to the stream provided. |
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/)(string, string) | Extracts the entry to the filesystem by the path provided. |
| [Open](../../aspose.zip.sevenzip/sevenziparchiveentry/open/)(string) | Opens the entry for extraction and provides a stream with entry content. |

## Events

| Name | Description |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip.sevenzip/sevenziparchiveentry/compressionprogressed/) | Raises when a portion of raw stream compressed. |

### See Also

* class [SevenZipArchiveEntry](../sevenziparchiveentry/)
* namespace [Aspose.Zip.SevenZip](../../aspose.zip.sevenzip/)
* assembly [Aspose.Zip](../../)


