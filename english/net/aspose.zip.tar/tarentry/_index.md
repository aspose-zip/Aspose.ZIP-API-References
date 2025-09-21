---
title: Class TarEntry
second_title: Aspose.ZIP for .NET API Reference
description: Aspose.Zip.Tar.TarEntry class. Represents single file within tar archive
type: docs
weight: 1010
url: /net/aspose.zip.tar/tarentry/
---
## TarEntry class

Represents single file within tar archive.

```csharp
public class TarEntry : IArchiveFileEntry
```

## Properties

| Name | Description |
| --- | --- |
| [IsDirectory](../../aspose.zip.tar/tarentry/isdirectory/) { get; } | Gets a value indicating whether the entry represents a directory. |
| [Length](../../aspose.zip.tar/tarentry/length/) { get; } | Get length of entry in bytes. |
| [ModificationTime](../../aspose.zip.tar/tarentry/modificationtime/) { get; } | Gets the modification time of the file or directory. |
| [Name](../../aspose.zip.tar/tarentry/name/) { get; set; } | Gets or sets a name of the entry within the archive. |
| [UncompressedSize](../../aspose.zip.tar/tarentry/uncompressedsize/) { get; } | Gets the size of an original file. |

## Methods

| Name | Description |
| --- | --- |
| [Extract](../../aspose.zip.tar/tarentry/extract/#extract_1)(Stream) | Extracts the entry to the stream provided. |
| [Extract](../../aspose.zip.tar/tarentry/extract/#extract)(string) | Extracts the entry to the filesystem by the path provided. |
| [Open](../../aspose.zip.tar/tarentry/open/)() | Opens the entry for extraction and provides a stream with entry content. |

### See Also

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Tar](../../aspose.zip.tar/)
* assembly [Aspose.Zip](../../)


