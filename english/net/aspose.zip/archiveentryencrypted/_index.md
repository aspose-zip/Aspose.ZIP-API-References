---
title: Class ArchiveEntryEncrypted
second_title: Aspose.ZIP for .NET API Reference
description: Aspose.Zip.ArchiveEntryEncrypted class. Zip entry that needs to be compressed with encryption or decompressed with decryption
type: docs
weight: 30
url: /net/aspose.zip/archiveentryencrypted/
---
## ArchiveEntryEncrypted class

Zip entry that needs to be compressed with encryption or decompressed with decryption.

```csharp
public sealed class ArchiveEntryEncrypted : ArchiveEntry
```

## Properties

| Name | Description |
| --- | --- |
| [Comment](../../aspose.zip/archiveentry/comment/) { get; } | Gets comment of the entry within archive. |
| [CompressedSize](../../aspose.zip/archiveentry/compressedsize/) { get; } | Gets size of the compressed file. |
| [CompressionSettings](../../aspose.zip/archiveentry/compressionsettings/) { get; } | Gets settings for compression or decompression. |
| [DataSource](../../aspose.zip/archiveentry/datasource/) { get; } | Source for the entry if the entry was added to the archive, not extracted. |
| [EncryptionSettings](../../aspose.zip/archiveentryencrypted/encryptionsettings/) { get; } | Gets settings for encryption or decryption. |
| [IsDirectory](../../aspose.zip/archiveentry/isdirectory/) { get; } | Gets a value indicating whether the entry represents a directory. |
| [ModificationTime](../../aspose.zip/archiveentry/modificationtime/) { get; set; } | Gets or sets last modified date and time. |
| [Name](../../aspose.zip/archiveentry/name/) { get; } | Gets name of the entry within the archive. |
| [UncompressedSize](../../aspose.zip/archiveentry/uncompressedsize/) { get; } | Gets size of the original file. |

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


