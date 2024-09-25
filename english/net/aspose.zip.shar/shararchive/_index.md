---
title: Class SharArchive
second_title: Aspose.ZIP for .NET API Reference
description: Aspose.Zip.Shar.SharArchive class. This class represents shar archive file
type: docs
weight: 790
url: /net/aspose.zip.shar/shararchive/
---
## SharArchive class

This class represents shar archive file.

```csharp
public class SharArchive : IDisposable
```

## Constructors

| Name | Description |
| --- | --- |
| [SharArchive](shararchive/#constructor)() | Initializes a new instance of the `SharArchive` class. |
| [SharArchive](shararchive/#constructor_1)(string) | Initializes a new instance of the `SharArchive` class prepared for decompressing. |

## Properties

| Name | Description |
| --- | --- |
| [Entries](../../aspose.zip.shar/shararchive/entries/) { get; } | Gets entries of [`SharEntry`](../sharentry/) type constituting the archive. |

## Methods

| Name | Description |
| --- | --- |
| [CreateEntries](../../aspose.zip.shar/shararchive/createentries/#createentries)(DirectoryInfo, bool) | Adds to the archive all the files and directories recursively in the directory given. |
| [CreateEntries](../../aspose.zip.shar/shararchive/createentries/#createentries_1)(string, bool) | Adds to the archive all the files and directories recursively in the directory given. |
| [CreateEntry](../../aspose.zip.shar/shararchive/createentry/#createentry_1)(string, Stream) | Create single entry within the archive. |
| [CreateEntry](../../aspose.zip.shar/shararchive/createentry/#createentry)(string, FileInfo, bool) | Create single entry within the archive. |
| [CreateEntry](../../aspose.zip.shar/shararchive/createentry/#createentry_2)(string, string, bool) | Create single entry within the archive. |
| [DeleteEntry](../../aspose.zip.shar/shararchive/deleteentry/#deleteentry_1)(int) | Removes the entry from the entries list by index. |
| [DeleteEntry](../../aspose.zip.shar/shararchive/deleteentry/#deleteentry)(SharEntry) | Removes the first occurrence of a specific entry from the entries list. |
| [Dispose](../../aspose.zip.shar/shararchive/dispose/)() | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [Save](../../aspose.zip.shar/shararchive/save/#save)(Stream) | Saves archive to the stream provided. |
| [Save](../../aspose.zip.shar/shararchive/save/#save_1)(string) | Saves archive to destination file provided. |

### See Also

* namespace [Aspose.Zip.Shar](../../aspose.zip.shar/)
* assembly [Aspose.Zip](../../)


