---
title: Class AlzEntryPlain
second_title: Aspose.ZIP for .NET API Reference
description: Aspose.Zip.Alz.AlzEntryPlain class. ALZ entry that needs to be decompressed without decryption
type: docs
weight: 50
url: /net/aspose.zip.alz/alzentryplain/
---
## AlzEntryPlain class

ALZ entry that needs to be decompressed without decryption.

```csharp
public sealed class AlzEntryPlain : AlzEntry
```

## Properties

| Name | Description |
| --- | --- |
| [CompressedSize](../../aspose.zip.alz/alzentry/compressedsize/) { get; } | Compressed size of the file data in bytes. |
| [IsDirectory](../../aspose.zip.alz/alzentry/isdirectory/) { get; } | Returns true if this entry represents a directory. |
| [Length](../../aspose.zip.alz/alzentry/length/) { get; } |  |
| [Name](../../aspose.zip.alz/alzentry/name/) { get; } | File name (without path). |
| [UncompressedSize](../../aspose.zip.alz/alzentry/uncompressedsize/) { get; } | Uncompressed size of the file data in bytes. |

## Methods

| Name | Description |
| --- | --- |
| [Extract](../../aspose.zip.alz/alzentry/extract/)(Stream, string) | Extracts the entry to the stream provided. |
| [Extract](../../aspose.zip.alz/alzentry/extract/)(string, string) | Extracts the entry to the filesystem by the path provided. |
| [Open](../../aspose.zip.alz/alzentry/open/)(string) | Opens the entry for extraction and provides a stream with decompressed entry content. |

### See Also

* class [AlzEntry](../alzentry/)
* namespace [Aspose.Zip.Alz](../../aspose.zip.alz/)
* assembly [Aspose.Zip](../../)


