---
title: Class CpioArchive
second_title: Aspose.ZIP for .NET API Reference
description: Aspose.Zip.Cpio.CpioArchive class. This class represents cpio archive file
type: docs
weight: 160
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
| [CpioArchive](cpioarchive/#constructor_1)(Stream) | Initializes a new instance of the `CpioArchive` class and composes entries list can be extracted from the archive. |
| [CpioArchive](cpioarchive/#constructor_2)(string) | Initializes a new instance of the `CpioArchive` class and composes entries list can be extracted from the archive. |

## Properties

| Name | Description |
| --- | --- |
| [Entries](../../aspose.zip.cpio/cpioarchive/entries/) { get; } | Gets entries of [`CpioEntry`](../cpioentry/) type constituting the archive. |

## Methods

| Name | Description |
| --- | --- |
| [CreateEntries](../../aspose.zip.cpio/cpioarchive/createentries/#createentries)(DirectoryInfo, bool) | Adds to the archive all the files and directories recursively in the directory given. |
| [CreateEntries](../../aspose.zip.cpio/cpioarchive/createentries/#createentries_1)(string, bool) | Adds to the archive all the files and directories recursively in the directory given. |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry_1)(string, Stream) | Create single entry within the archive. |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry)(string, FileInfo, bool) | Create single entry within the archive. |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry_2)(string, string, bool) | Create single entry within the archive. |
| [DeleteEntry](../../aspose.zip.cpio/cpioarchive/deleteentry/#deleteentry)(CpioEntry) | Removes the first occurrence of a specific entry from the entries list. |
| [DeleteEntry](../../aspose.zip.cpio/cpioarchive/deleteentry/#deleteentry_1)(int) | Removes the entry from the entries list by index. |
| [Dispose](../../aspose.zip.cpio/cpioarchive/dispose/)() | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [ExtractToDirectory](../../aspose.zip.cpio/cpioarchive/extracttodirectory/)(string) | Extracts all the files in the archive to the directory provided. |
| [Save](../../aspose.zip.cpio/cpioarchive/save/#save)(Stream, CpioFormat) | Saves archive to the stream provided. |
| [Save](../../aspose.zip.cpio/cpioarchive/save/#save_1)(string, CpioFormat) | Saves archive to destination file provided. |
| [SaveGzipped](../../aspose.zip.cpio/cpioarchive/savegzipped/#savegzipped)(Stream, CpioFormat) | Saves archive to the stream with gzip compression. |
| [SaveGzipped](../../aspose.zip.cpio/cpioarchive/savegzipped/#savegzipped_1)(string, CpioFormat) | Saves archive to the file by path with gzip compression. |
| [SaveXzCompressed](../../aspose.zip.cpio/cpioarchive/savexzcompressed/#savexzcompressed)(Stream, CpioFormat, XzArchiveSettings) | Saves archive to the stream with xz compression. |
| [SaveXzCompressed](../../aspose.zip.cpio/cpioarchive/savexzcompressed/#savexzcompressed_1)(string, CpioFormat, XzArchiveSettings) | Saves archive to the path by path with xz compression. |

### See Also

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Cpio](../../aspose.zip.cpio/)
* assembly [Aspose.Zip](../../)


