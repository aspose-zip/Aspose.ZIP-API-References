---
title: Class XarFileEntry
second_title: Aspose.ZIP for .NET API Reference
description: Aspose.Zip.Xar.XarFileEntry class. Represents file entry within xar archive
type: docs
weight: 920
url: /net/aspose.zip.xar/xarfileentry/
---
## XarFileEntry class

Represents file entry within xar archive.

```csharp
public sealed class XarFileEntry : XarEntry, IArchiveFileEntry
```

## Properties

| Name | Description |
| --- | --- |
| [CreationTime](../../aspose.zip.xar/xarentry/creationtime/) { get; } | Gets the creation time of the file or directory. |
| [FullPath](../../aspose.zip.xar/xarentry/fullpath/) { get; } | Gets full path of the entry within archive. |
| [IsDirectory](../../aspose.zip.xar/xarentry/isdirectory/) { get; } | Gets a value indicating whether the entry represents directory. |
| [LastAccessTime](../../aspose.zip.xar/xarentry/lastaccesstime/) { get; } | Gets the last access time of the file or directory. |
| [LastWriteTime](../../aspose.zip.xar/xarentry/lastwritetime/) { get; } | Gets the modification time of the file or directory. |
| [Length](../../aspose.zip.xar/xarfileentry/length/) { get; } | Gets the length of the entry in bytes. |
| [Name](../../aspose.zip.xar/xarentry/name/) { get; } | Gets name of the entry within archive. |
| [Parent](../../aspose.zip.xar/xarentry/parent/) { get; } | Gets the parent directory the entry belongs to. |

## Methods

| Name | Description |
| --- | --- |
| [Extract](../../aspose.zip.xar/xarfileentry/extract/#extract_1)(Stream) | Extracts the entry to the stream provided. |
| [Extract](../../aspose.zip.xar/xarfileentry/extract/#extract)(string) | Extracts the entry to the filesystem by the path provided. |
| [Open](../../aspose.zip.xar/xarfileentry/open/)() | Opens the entry for extraction and provides a stream with entry content. |
| override [ToString](../../aspose.zip.xar/xarentry/tostring/)() |  |

### See Also

* class [XarEntry](../xarentry/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Xar](../../aspose.zip.xar/)
* assembly [Aspose.Zip](../../)


