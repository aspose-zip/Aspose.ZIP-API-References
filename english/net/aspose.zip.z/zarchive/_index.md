---
title: Class ZArchive
second_title: Aspose.ZIP for .NET API Reference
description: Aspose.Zip.Z.ZArchive class. This class represents a Z compress archive file. Use it to compose or extract Z archives
type: docs
weight: 1270
url: /net/aspose.zip.z/zarchive/
---
## ZArchive class

This class represents a Z (compress) archive file. Use it to compose or extract Z archives.

```csharp
public class ZArchive : IArchive, IArchiveFileEntry
```

## Constructors

| Name | Description |
| --- | --- |
| [ZArchive](zarchive/#constructor)() | Initializes a new instance of the `ZArchive` class prepared for compressing. |
| [ZArchive](zarchive/#constructor_1)(Stream, ZArchiveLoadOptions) | Initializes a new instance of the `ZArchive` class prepared for decompressing. |
| [ZArchive](zarchive/#constructor_2)(string, ZArchiveLoadOptions) | Initializes a new instance of the `ZArchive` class prepared for decompressing. |

## Methods

| Name | Description |
| --- | --- |
| [Dispose](../../aspose.zip.z/zarchive/dispose/)() | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [Extract](../../aspose.zip.z/zarchive/extract/#extract_1)(FileInfo) | Extracts Z archive to a file. |
| [Extract](../../aspose.zip.z/zarchive/extract/#extract_2)(Stream) | Extracts Z archive to a stream. |
| [Extract](../../aspose.zip.z/zarchive/extract/#extract)(string) | Extracts Z archive to a file by path. |
| [ExtractToDirectory](../../aspose.zip.z/zarchive/extracttodirectory/)(string) | Extracts content of the archive to the directory provided. |
| [Save](../../aspose.zip.z/zarchive/save/#save)(Stream, ZArchiveSaveOptions) | Saves xz archive to the stream provided. |
| [Save](../../aspose.zip.z/zarchive/save/#save_1)(string, ZArchiveSaveOptions) | Saves Z archive to the destination file provided. |
| [SetSource](../../aspose.zip.z/zarchive/setsource/#setsource)(FileInfo) | Sets the content to be compressed within the archive. |
| [SetSource](../../aspose.zip.z/zarchive/setsource/#setsource_1)(Stream) | Sets the content to be compressed within the archive. |
| [SetSource](../../aspose.zip.z/zarchive/setsource/#setsource_2)(string) | Sets the content to be compressed within the archive. |

## Remarks

See https://docs.fileformat.com/compression/z/

### See Also

* interface [IArchive](../../aspose.zip/iarchive/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Z](../../aspose.zip.z/)
* assembly [Aspose.Zip](../../)


