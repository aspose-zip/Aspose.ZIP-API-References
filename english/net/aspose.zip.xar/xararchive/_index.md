---
title: Class XarArchive
second_title: Aspose.ZIP for .NET API Reference
description: Aspose.Zip.Xar.XarArchive class. This class represents xar archive file
type: docs
weight: 850
url: /net/aspose.zip.xar/xararchive/
---
## XarArchive class

This class represents xar archive file.

```csharp
public class XarArchive : IArchive
```

## Constructors

| Name | Description |
| --- | --- |
| [XarArchive](xararchive/#constructor_1)(Stream) | Initializes a new instance of the `XarArchive` class and composes entries list can be extracted from the archive. |
| [XarArchive](xararchive/#constructor_2)(string) | Initializes a new instance of the `XarArchive` class and composes entries list can be extracted from the archive. |
| [XarArchive](xararchive/#constructor)(XarCompressionSettings) | Initializes a new instance of the `XarArchive` class. |

## Properties

| Name | Description |
| --- | --- |
| [Entries](../../aspose.zip.xar/xararchive/entries/) { get; } | Gets entries of [`XarEntry`](../xarentry/) type constituting the archive. |

## Methods

| Name | Description |
| --- | --- |
| [CreateEntries](../../aspose.zip.xar/xararchive/createentries/#createentries)(DirectoryInfo, bool, XarCompressionSettings) | Adds to the archive all the files and directories recursively in the directory given. |
| [CreateEntries](../../aspose.zip.xar/xararchive/createentries/#createentries_1)(string, bool, XarCompressionSettings) | Adds to the archive all the files and directories recursively in the directory given. |
| [CreateEntry](../../aspose.zip.xar/xararchive/createentry/#createentry_1)(string, Stream, XarCompressionSettings) | Create single entry within the archive. |
| [CreateEntry](../../aspose.zip.xar/xararchive/createentry/#createentry)(string, FileInfo, bool, XarCompressionSettings) | Create single entry within the archive. |
| [CreateEntry](../../aspose.zip.xar/xararchive/createentry/#createentry_2)(string, string, bool, XarCompressionSettings) | Create single entry within the archive. |
| [DeleteEntry](../../aspose.zip.xar/xararchive/deleteentry/)(XarEntry) | Removes the first occurrence of a specific entry from the entries list. |
| [Dispose](../../aspose.zip.xar/xararchive/dispose/)() | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [ExtractToDirectory](../../aspose.zip.xar/xararchive/extracttodirectory/)(string) | Extracts all the files in the archive to the directory provided. |
| [Save](../../aspose.zip.xar/xararchive/save/#save)(Stream) | Saves archive to the stream provided. |
| [Save](../../aspose.zip.xar/xararchive/save/#save_1)(string) | Saves archive to destination file provided. |

### See Also

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Xar](../../aspose.zip.xar/)
* assembly [Aspose.Zip](../../)


