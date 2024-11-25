---
title: Class LhaArchive
second_title: Aspose.ZIP for .NET API Reference
description: Aspose.Zip.Lha.LhaArchive class. This class represents LHA .lzh archive file
type: docs
weight: 340
url: /net/aspose.zip.lha/lhaarchive/
---
## LhaArchive class

This class represents LHA (.lzh) archive file.

```csharp
public class LhaArchive : IArchive
```

## Constructors

| Name | Description |
| --- | --- |
| [LhaArchive](lhaarchive/#constructor)(Stream) | Initializes a new instance of the `LhaArchive` class and composes entries list can be extracted from the archive. |
| [LhaArchive](lhaarchive/#constructor_1)(string) | Initializes a new instance of the `LhaArchive` class and composes entries list can be extracted from the archive. |

## Properties

| Name | Description |
| --- | --- |
| [Directories](../../aspose.zip.lha/lhaarchive/directories/) { get; } | Gets directory entries of [`LhaDirectoryEntry`](../lhadirectoryentry/) type constituting the archive. |
| [Entries](../../aspose.zip.lha/lhaarchive/entries/) { get; } | Gets file entries of [`LhaArchiveEntry`](../lhaarchiveentry/) type constituting the archive. |

## Methods

| Name | Description |
| --- | --- |
| [Dispose](../../aspose.zip.lha/lhaarchive/dispose/)() |  |
| [ExtractToDirectory](../../aspose.zip.lha/lhaarchive/extracttodirectory/)(string) | Extracts all the files and directories in the archive to the directory provided. |

## Remarks

Only following compression methods are supported:

**Method**

**Explanation**

**lh0**

Uncompressed

**lh4**

8 KiB sliding dictionary and static Huffman

**lh5**

16 KiB sliding dictionary and static Huffman

**lh6**

64 KiB sliding dictionary and static Huffman

**lh7**

128 KiB sliding dictionary and static Huffman

**lhx**

1 Mib sliding dictionary and static Huffman

**lhd**

Directory

### See Also

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Lha](../../aspose.zip.lha/)
* assembly [Aspose.Zip](../../)


