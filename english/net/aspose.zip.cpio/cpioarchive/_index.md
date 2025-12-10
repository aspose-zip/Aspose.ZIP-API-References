---
title: Class CpioArchive
second_title: Aspose.ZIP for .NET API Reference
description: Aspose.Zip.Cpio.CpioArchive class. This class represents cpio archive file
type: docs
weight: 260
url: /net/aspose.zip.cpio/cpioarchive/
---
## CpioArchive class

This class represents cpio archive file.

```csharp
public class CpioArchive : IArchive
```

## Constructors

| Name | Description |
| --- | --- |
| [CpioArchive](cpioarchive/#constructor)() | Initializes a new instance of the `CpioArchive` class. |
| [CpioArchive](cpioarchive/#constructor_1)(Stream) | Initializes a new instance of the `CpioArchive` class and composes an entry list can be extracted from the archive. |
| [CpioArchive](cpioarchive/#constructor_2)(string) | Initializes a new instance of the `CpioArchive` class and composes an entry list can be extracted from the archive. |

## Properties

| Name | Description |
| --- | --- |
| [Entries](../../aspose.zip.cpio/cpioarchive/entries/) { get; } | Gets entries of [`CpioEntry`](../cpioentry/) type constituting the archive. |

## Methods

| Name | Description |
| --- | --- |
| [CreateEntries](../../aspose.zip.cpio/cpioarchive/createentries/#createentries)(DirectoryInfo, bool) | Adds to the archive all the files and directories recursively in the directory given. |
| [CreateEntries](../../aspose.zip.cpio/cpioarchive/createentries/#createentries_1)(string, bool) | Adds to the archive all the files and directories recursively in the directory given. |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry_1)(string, Stream) | Create a single entry within the archive. |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry)(string, FileInfo, bool) | Create a single entry within the archive. |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry_2)(string, string, bool) | Create a single entry within the archive. |
| [DeleteEntry](../../aspose.zip.cpio/cpioarchive/deleteentry/#deleteentry)(CpioEntry) | Removes the first occurrence of a specific entry from the entry list. |
| [DeleteEntry](../../aspose.zip.cpio/cpioarchive/deleteentry/#deleteentry_1)(int) | Removes the entry from the entry list by index. |
| [Dispose](../../aspose.zip.cpio/cpioarchive/dispose/)() | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [ExtractToDirectory](../../aspose.zip.cpio/cpioarchive/extracttodirectory/)(string) | Extracts all the files in the archive to the directory provided. |
| [Save](../../aspose.zip.cpio/cpioarchive/save/#save)(Stream, CpioFormat) | Saves archive to the stream provided. |
| [Save](../../aspose.zip.cpio/cpioarchive/save/#save_1)(string, CpioFormat) | Saves archive to a destination file provided. |
| [SaveGzipped](../../aspose.zip.cpio/cpioarchive/savegzipped/#savegzipped)(Stream, CpioFormat) | Saves archive to the stream with gzip compression. |
| [SaveGzipped](../../aspose.zip.cpio/cpioarchive/savegzipped/#savegzipped_1)(string, CpioFormat) | Saves archive to the file by path with gzip compression. |
| [SaveLzipped](../../aspose.zip.cpio/cpioarchive/savelzipped/#savelzipped)(Stream, CpioFormat) | Saves archive to the stream with lzip compression. |
| [SaveLzipped](../../aspose.zip.cpio/cpioarchive/savelzipped/#savelzipped_1)(string, CpioFormat) | Saves archive to the file by path with lzip compression. |
| [SaveLZMACompressed](../../aspose.zip.cpio/cpioarchive/savelzmacompressed/#savelzmacompressed)(Stream, CpioFormat) | Saves the archive to the stream with LZMA compression. |
| [SaveLZMACompressed](../../aspose.zip.cpio/cpioarchive/savelzmacompressed/#savelzmacompressed_1)(string, CpioFormat) | Saves the archive to the file by path with lzma compression. |
| [SaveXzCompressed](../../aspose.zip.cpio/cpioarchive/savexzcompressed/#savexzcompressed)(Stream, CpioFormat, XzArchiveSettings) | Saves archive to the stream with xz compression. |
| [SaveXzCompressed](../../aspose.zip.cpio/cpioarchive/savexzcompressed/#savexzcompressed_1)(string, CpioFormat, XzArchiveSettings) | Saves archive to the path by path with xz compression. |
| [SaveZCompressed](../../aspose.zip.cpio/cpioarchive/savezcompressed/#savezcompressed)(Stream, CpioFormat) | Saves archive to the stream with Z compression. |
| [SaveZCompressed](../../aspose.zip.cpio/cpioarchive/savezcompressed/#savezcompressed_1)(string, CpioFormat) | Saves archive to the path by path with Z compression. |
| [SaveZstandard](../../aspose.zip.cpio/cpioarchive/savezstandard/#savezstandard)(Stream, CpioFormat) | Saves archive to the stream with Zstandard compression. |
| [SaveZstandard](../../aspose.zip.cpio/cpioarchive/savezstandard/#savezstandard_1)(string, CpioFormat) | Saves archive to the file by path with Zstandard compression. |

### See Also

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Cpio](../../aspose.zip.cpio/)
* assembly [Aspose.Zip](../../)


