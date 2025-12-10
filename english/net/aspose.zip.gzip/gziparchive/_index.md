---
title: Class GzipArchive
second_title: Aspose.ZIP for .NET API Reference
description: Aspose.Zip.Gzip.GzipArchive class. This class represents a gzip archive file. Use it to compose or extract gzip archives
type: docs
weight: 320
url: /net/aspose.zip.gzip/gziparchive/
---
## GzipArchive class

This class represents a gzip archive file. Use it to compose or extract gzip archives.

```csharp
public class GzipArchive : IArchive, IArchiveFileEntry
```

## Constructors

| Name | Description |
| --- | --- |
| [GzipArchive](gziparchive/#constructor)() | Initializes a new instance of the `GzipArchive` class prepared for compressing. |
| [GzipArchive](gziparchive/#constructor_2)(Stream, bool) | Initializes a new instance of the `GzipArchive` class prepared for decompressing. |
| [GzipArchive](gziparchive/#constructor_1)(Stream, GzipLoadOptions) | Initializes a new instance of the `GzipArchive` class prepared for decompressing. |
| [GzipArchive](gziparchive/#constructor_4)(string, bool) | Initializes a new instance of the `GzipArchive` class prepared for decompressing. |
| [GzipArchive](gziparchive/#constructor_3)(string, GzipLoadOptions) | Initializes a new instance of the `GzipArchive` class prepared for decompressing. |

## Properties

| Name | Description |
| --- | --- |
| [Name](../../aspose.zip.gzip/gziparchive/name/) { get; } | Name of the original file. |
| [UncompressedSize](../../aspose.zip.gzip/gziparchive/uncompressedsize/) { get; } | Gets size of an original file. |

## Methods

| Name | Description |
| --- | --- |
| [Dispose](../../aspose.zip.gzip/gziparchive/dispose/)() | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [Extract](../../aspose.zip.gzip/gziparchive/extract/#extract_1)(Stream) | Extracts the archive to the stream provided. |
| [Extract](../../aspose.zip.gzip/gziparchive/extract/#extract)(string) | Extracts the archive to the file by path. |
| [ExtractToDirectory](../../aspose.zip.gzip/gziparchive/extracttodirectory/)(string) | Extracts content of the archive to the directory provided. |
| [Open](../../aspose.zip.gzip/gziparchive/open/)() | Opens the archive for extraction and provides a stream with archive content. |
| [Save](../../aspose.zip.gzip/gziparchive/save/#save)(Stream) | Saves archive to the stream provided. |
| [Save](../../aspose.zip.gzip/gziparchive/save/#save_1)(string) | Saves archive to the destination file provided. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_1)(FileInfo) | Sets the content to be compressed within the archive. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_2)(Stream) | Sets the content to be compressed within the archive. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_3)(string) | Sets the content to be compressed within the archive. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource)(TarArchive) | Sets the content to be compressed within the archive. |

## Remarks

Gzip compression algorithm is based on the DEFLATE algorithm, which is a combination of LZ77 and Huffman coding.

### See Also

* interface [IArchive](../../aspose.zip/iarchive/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Gzip](../../aspose.zip.gzip/)
* assembly [Aspose.Zip](../../)


