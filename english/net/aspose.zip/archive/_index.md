---
title: Class Archive
second_title: Aspose.ZIP for .NET API Reference
description: Aspose.Zip.Archive class. This class represents zip archive file. Use it to compose extract or update zip archives
type: docs
weight: 30
url: /net/aspose.zip/archive/
---
## Archive class

This class represents zip archive file. Use it to compose, extract, or update zip archives.

```csharp
public class Archive : IArchive
```

## Constructors

| Name | Description |
| --- | --- |
| [Archive](archive/#constructor)(ArchiveEntrySettings) | Initializes a new instance of the `Archive` class with optional settings for its entries. |
| [Archive](archive/#constructor_1)(Stream, ArchiveLoadOptions, ArchiveEntrySettings) | Initializes a new instance of the `Archive` class and composes entries list can be extracted from the archive. |
| [Archive](archive/#constructor_2)(string, ArchiveLoadOptions, ArchiveEntrySettings) | Initializes a new instance of the `Archive` class and composes entries list can be extracted from the archive. |
| [Archive](archive/#constructor_3)(string, string[], ArchiveLoadOptions) | Initializes a new instance of the `Archive` class from multi-volume zip archive and composes entries list can be extracted from the archive. |

## Properties

| Name | Description |
| --- | --- |
| [Entries](../../aspose.zip/archive/entries/) { get; } | Gets entries of [`ArchiveEntry`](../archiveentry/) type constituting the archive. |
| [NewEntrySettings](../../aspose.zip/archive/newentrysettings/) { get; } | Compression and encryption settings used for newly added [`ArchiveEntry`](../archiveentry/) items. |

## Methods

| Name | Description |
| --- | --- |
| [CreateEntries](../../aspose.zip/archive/createentries/#createentries)(DirectoryInfo, bool) | Adds to the archive all files and directories recursively in the directory given. |
| [CreateEntries](../../aspose.zip/archive/createentries/#createentries_1)(string, bool) | Adds to the archive all files and directories recursively in the directory given. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry)(string, Func&lt;Stream&gt;, ArchiveEntrySettings) | Create single entry within the archive. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_2)(string, Stream, ArchiveEntrySettings) | Create single entry within the archive. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_1)(string, FileInfo, bool, ArchiveEntrySettings) | Create single entry within the archive. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_3)(string, Stream, ArchiveEntrySettings, FileSystemInfo) | Create single entry within the archive. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_4)(string, string, bool, ArchiveEntrySettings) | Create single entry within the archive. |
| [DeleteEntry](../../aspose.zip/archive/deleteentry/#deleteentry)(ArchiveEntry) | Removes the first occurrence of a specific entry from the entries list. |
| [DeleteEntry](../../aspose.zip/archive/deleteentry/#deleteentry_1)(int) | Removes the entry from the entries list by index. |
| [Dispose](../../aspose.zip/archive/dispose/)() | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [ExtractToDirectory](../../aspose.zip/archive/extracttodirectory/)(string) | Extracts all the files in the archive to the directory provided. |
| [Save](../../aspose.zip/archive/save/#save)(Stream, ArchiveSaveOptions) | Saves archive to the stream provided. |
| [Save](../../aspose.zip/archive/save/#save_1)(string, ArchiveSaveOptions) | Saves archive to destination file provided. |
| [SaveSplit](../../aspose.zip/archive/savesplit/)(string, SplitArchiveSaveOptions) | Saves multi-volume archive to destination directory provided. |

### See Also

* interface [IArchive](../iarchive/)
* namespace [Aspose.Zip](../../aspose.zip/)
* assembly [Aspose.Zip](../../)


