---
title: Class CabArchive
second_title: Aspose.ZIP for .NET API Reference
description: Aspose.Zip.Cab.CabArchive class. This class represents a CAB archive file
type: docs
weight: 160
url: /net/aspose.zip.cab/cabarchive/
---
## CabArchive class

This class represents a CAB archive file.

```csharp
public class CabArchive : IArchive
```

## Constructors

| Name | Description |
| --- | --- |
| [CabArchive](cabarchive/#constructor)(CabEntrySettings) | Initializes a new instance of the `CabArchive` class prepared for compressing. |
| [CabArchive](cabarchive/#constructor_1)(Stream, CabLoadOptions) | Initializes a new instance of the `CabArchive` class and composes an entry list can be extracted from the archive. |
| [CabArchive](cabarchive/#constructor_2)(string, CabLoadOptions) | Initializes a new instance of the `CabArchive` class and composes an entry list can be extracted from the archive. |

## Properties

| Name | Description |
| --- | --- |
| [Entries](../../aspose.zip.cab/cabarchive/entries/) { get; } | Gets entries of [`CabEntry`](../cabentry/) type constituting the archive. |

## Methods

| Name | Description |
| --- | --- |
| [CreateEntries](../../aspose.zip.cab/cabarchive/createentries/#createentries)(DirectoryInfo, bool) | Adds to the archive all files, recursively, from the specified directory. |
| [CreateEntries](../../aspose.zip.cab/cabarchive/createentries/#createentries_1)(string, bool) | Adds to the archive all files recursively from the specified directory path. |
| [CreateEntry](../../aspose.zip.cab/cabarchive/createentry/#createentry)(string, FileInfo, CabEntrySettings) | Create a single entry within the archive. |
| [CreateEntry](../../aspose.zip.cab/cabarchive/createentry/#createentry_1)(string, Stream, CabEntrySettings) | Create a single entry within the archive. |
| [CreateEntry](../../aspose.zip.cab/cabarchive/createentry/#createentry_2)(string, string, CabEntrySettings) | Create a single entry within the archive. |
| [Dispose](../../aspose.zip.cab/cabarchive/dispose/)() | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [ExtractToDirectory](../../aspose.zip.cab/cabarchive/extracttodirectory/)(string) | Extracts all the files in the archive to the directory provided. |
| [Save](../../aspose.zip.cab/cabarchive/save/#save)(Stream, CabSaveOptions) | Saves archive to the stream provided. |
| [Save](../../aspose.zip.cab/cabarchive/save/#save_1)(string, CabSaveOptions) | Saves archive to the destination file provided. |

### See Also

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Cab](../../aspose.zip.cab/)
* assembly [Aspose.Zip](../../)


