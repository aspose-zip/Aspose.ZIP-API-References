---
title: Class WimFileEntry
second_title: Aspose.ZIP for .NET API Reference
description: Aspose.Zip.Wim.WimFileEntry class. Represents a single file within wim archive
type: docs
weight: 1040
url: /net/aspose.zip.wim/wimfileentry/
---
## WimFileEntry class

Represents a single file within wim archive.

```csharp
public sealed class WimFileEntry : WimEntry, IArchiveFileEntry
```

## Properties

| Name | Description |
| --- | --- |
| [AlternateDataStreams](../../aspose.zip.wim/wimentry/alternatedatastreams/) { get; } | Gets the names of the alternate data streams for a file or directory. |
| [Archive](../../aspose.zip.wim/wimentry/archive/) { get; } | Gets the archive the entry belongs to. |
| [ChangeTime](../../aspose.zip.wim/wimentry/changetime/) { get; } | Gets the last time the file or directory was changed. |
| [CreationTime](../../aspose.zip.wim/wimentry/creationtime/) { get; } | Gets the creation time of the file or directory. |
| [FileAttributes](../../aspose.zip.wim/wimentry/fileattributes/) { get; } | Gets the file or directory attributes. |
| [FullPath](../../aspose.zip.wim/wimentry/fullpath/) { get; } | Gets a full path of the entry within the image. |
| [HardLink](../../aspose.zip.wim/wimentry/hardlink/) { get; } | Gets the hardlink id of the file or directory. |
| [HasHardLinks](../../aspose.zip.wim/wimentry/hashardlinks/) { get; } | Gets whether the file or directory is known by other names. |
| [Image](../../aspose.zip.wim/wimentry/image/) { get; } | Gets the image the entry belongs to. |
| [IsDirectory](../../aspose.zip.wim/wimentry/isdirectory/) { get; } | Gets a value indicating whether the entry represents a directory. |
| [LastAccessTime](../../aspose.zip.wim/wimentry/lastaccesstime/) { get; } | Gets the last access time of the file or directory. |
| [Length](../../aspose.zip.wim/wimfileentry/length/) { get; } | Gets the length of the entry in bytes. |
| [ModificationTime](../../aspose.zip.wim/wimentry/modificationtime/) { get; } | Gets the modification time of the file or directory. |
| [Name](../../aspose.zip.wim/wimentry/name/) { get; } | Gets name of the entry within the image. |
| [Parent](../../aspose.zip.wim/wimentry/parent/) { get; } | Gets the parent directory the entry belongs to. |
| [ShortName](../../aspose.zip.wim/wimentry/shortname/) { get; } | Gets short name of the entry within the image. |

## Methods

| Name | Description |
| --- | --- |
| [Extract](../../aspose.zip.wim/wimfileentry/extract/#extract_1)(Stream) | Extracts the entry to the stream provided. |
| [Extract](../../aspose.zip.wim/wimfileentry/extract/#extract)(string) | Extracts the entry to the filesystem by the path provided. |
| [Open](../../aspose.zip.wim/wimfileentry/open/)() | Opens the entry for extraction and provides a stream with entry content. |
| override [ToString](../../aspose.zip.wim/wimentry/tostring/)() |  |

### See Also

* class [WimEntry](../wimentry/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Wim](../../aspose.zip.wim/)
* assembly [Aspose.Zip](../../)


