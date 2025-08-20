---
title: Class SevenZipArchiveEntry
second_title: Aspose.ZIP for .NET API Reference
description: Aspose.Zip.SevenZip.SevenZipArchiveEntry class. Represents a single file within 7z archive
type: docs
weight: 900
url: /net/aspose.zip.sevenzip/sevenziparchiveentry/
---
## SevenZipArchiveEntry class

Represents a single file within 7z archive.

```csharp
public abstract class SevenZipArchiveEntry : IArchiveFileEntry
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
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/#extract_1)(Stream, string) | Extracts the entry to the stream provided. |
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/#extract)(string, string) | Extracts the entry to the filesystem by the path provided. |
| [Open](../../aspose.zip.sevenzip/sevenziparchiveentry/open/)(string) | Opens the entry for extraction and provides a stream with entry content. |

## Events

| Name | Description |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip.sevenzip/sevenziparchiveentry/compressionprogressed/) | Raises when a portion of raw stream compressed. |

## Remarks

Cast an `SevenZipArchiveEntry` instance to [`SevenZipArchiveEntryEncrypted`](../sevenziparchiveentryencrypted/) to determine whether the entry encrypted or not.

### See Also

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.SevenZip](../../aspose.zip.sevenzip/)
* assembly [Aspose.Zip](../../)


