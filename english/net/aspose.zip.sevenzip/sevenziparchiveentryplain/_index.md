---
title: Class SevenZipArchiveEntryPlain
second_title: Aspose.ZIP for .NET API Reference
description: Aspose.Zip.SevenZip.SevenZipArchiveEntryPlain class. SevenZip entry that needs to be compressed without encryption or decompressed without decryption
type: docs
weight: 830
url: /net/aspose.zip.sevenzip/sevenziparchiveentryplain/
---
## SevenZipArchiveEntryPlain class

SevenZip entry that needs to be compressed without encryption or decompressed without decryption.

```csharp
public class SevenZipArchiveEntryPlain : SevenZipArchiveEntry
```

## Properties

| Name | Description |
| --- | --- |
| [CompressedSize](../../aspose.zip.sevenzip/sevenziparchiveentry/compressedsize/) { get; } | Gets the size of a compressed file. |
| [CompressionSettings](../../aspose.zip.sevenzip/sevenziparchiveentry/compressionsettings/) { get; } | Gets settings for compression or decompression. |
| [IsDirectory](../../aspose.zip.sevenzip/sevenziparchiveentry/isdirectory/) { get; } | Gets a value indicating whether the entry represents a directory. |
| [ModificationTime](../../aspose.zip.sevenzip/sevenziparchiveentry/modificationtime/) { get; } | Gets last modified date and time. |
| [Name](../../aspose.zip.sevenzip/sevenziparchiveentry/name/) { get; } | Gets name of the entry within the archive. |
| [UncompressedSize](../../aspose.zip.sevenzip/sevenziparchiveentry/uncompressedsize/) { get; } | Gets size of an original file. |

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


