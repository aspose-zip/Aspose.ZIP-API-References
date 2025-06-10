---
title: Class Bzip2Archive
second_title: Aspose.ZIP for .NET API Reference
description: Aspose.Zip.Bzip2.Bzip2Archive class. This class represents bzip2 archive file. Use it to compose or extract bzip2 archives
type: docs
weight: 130
url: /net/aspose.zip.bzip2/bzip2archive/
---
## Bzip2Archive class

This class represents bzip2 archive file. Use it to compose or extract bzip2 archives.

```csharp
public class Bzip2Archive : IArchive, IArchiveFileEntry
```

## Constructors

| Name | Description |
| --- | --- |
| [Bzip2Archive](bzip2archive/#constructor)() | Initializes a new instance of the `Bzip2Archive` class prepared for compressing. |
| [Bzip2Archive](bzip2archive/#constructor_1)(Stream, Bzip2LoadOptions) | Initializes a new instance of the `Bzip2Archive` class prepared for decompressing. |
| [Bzip2Archive](bzip2archive/#constructor_2)(string, Bzip2LoadOptions) | Initializes a new instance of the `Bzip2Archive` class prepared for decompressing. |

## Methods

| Name | Description |
| --- | --- |
| [Dispose](../../aspose.zip.bzip2/bzip2archive/dispose/)() | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [Extract](../../aspose.zip.bzip2/bzip2archive/extract/#extract_1)(Stream) | Extracts the archive to the stream provided. |
| [Extract](../../aspose.zip.bzip2/bzip2archive/extract/#extract)(string) | Extracts the archive to the file by path. |
| [ExtractToDirectory](../../aspose.zip.bzip2/bzip2archive/extracttodirectory/)(string) | Extracts content of the archive to the directory provided. |
| [Open](../../aspose.zip.bzip2/bzip2archive/open/)() | Opens the archive for extraction and provides a stream with archive content. |
| [Save](../../aspose.zip.bzip2/bzip2archive/save/#save)(Stream, Bzip2SaveOptions) | Saves archive to the stream provided. |
| [Save](../../aspose.zip.bzip2/bzip2archive/save/#save_1)(string, Bzip2SaveOptions) | Saves archive to a destination file provided. |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource_2)(FileInfo) | Sets the content to be compressed within the archive. |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource_3)(Stream) | Sets the content to be compressed within the archive. |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource_4)(string) | Sets the content to be compressed within the archive. |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource)(CpioArchive, CpioFormat) | Sets the content to be compressed within the archive. |
| [SetSource](../../aspose.zip.bzip2/bzip2archive/setsource/#setsource_1)(TarArchive, TarFormat) | Sets the content to be compressed within the archive. |

## Remarks

bzip2 compresses files using the Burrows-Wheeler block sorting text compression algorithm, and Huffman coding. See more: https://en.wikipedia.org/wiki/Bzip2

### See Also

* interface [IArchive](../../aspose.zip/iarchive/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Bzip2](../../aspose.zip.bzip2/)
* assembly [Aspose.Zip](../../)


