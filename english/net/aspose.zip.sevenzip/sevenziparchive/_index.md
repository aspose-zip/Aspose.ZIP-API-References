---
title: Class SevenZipArchive
second_title: Aspose.ZIP for .NET API Reference
description: Aspose.Zip.SevenZip.SevenZipArchive class. This class represents 7z archive file. Use it to compose and extract 7z archives
type: docs
weight: 750
url: /net/aspose.zip.sevenzip/sevenziparchive/
---
## SevenZipArchive class

This class represents 7z archive file. Use it to compose and extract 7z archives.

```csharp
public class SevenZipArchive : IArchive
```

## Constructors

| Name | Description |
| --- | --- |
| [SevenZipArchive](sevenziparchive/#constructor)(SevenZipEntrySettings) | Initializes a new instance of the `SevenZipArchive` class with optional settings for its entries. |
| [SevenZipArchive](sevenziparchive/#constructor_1)(Stream, string) | Initializes a new instance of the `SevenZipArchive` class and composes entries list can be extracted from the archive. |
| [SevenZipArchive](sevenziparchive/#constructor_2)(string, string) | Initializes a new instance of the `SevenZipArchive` class and composes entries list can be extracted from the archive. |
| [SevenZipArchive](sevenziparchive/#constructor_3)(string[], string) | Initializes a new instance of the `SevenZipArchive` class from multi-volume 7z archive and composes entries list can be extracted from the archive. |

## Properties

| Name | Description |
| --- | --- |
| [Entries](../../aspose.zip.sevenzip/sevenziparchive/entries/) { get; } | Gets entries of [`SevenZipArchiveEntry`](../sevenziparchiveentry/) type constituting the archive. |
| [NewEntrySettings](../../aspose.zip.sevenzip/sevenziparchive/newentrysettings/) { get; } | Compression and encryption settings used for newly added [`SevenZipArchiveEntry`](../sevenziparchiveentry/) items. |

## Methods

| Name | Description |
| --- | --- |
| [CreateEntries](../../aspose.zip.sevenzip/sevenziparchive/createentries/#createentries)(DirectoryInfo, bool) | Adds to the archive all files and directories recursively in the directory given. |
| [CreateEntries](../../aspose.zip.sevenzip/sevenziparchive/createentries/#createentries_1)(string, bool) | Adds to the archive all files and directories recursively in the directory given. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_1)(string, Stream, SevenZipEntrySettings) | Create single entry within the archive. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry)(string, FileInfo, bool, SevenZipEntrySettings) | Create single entry within the archive. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_2)(string, Stream, SevenZipEntrySettings, FileSystemInfo) | Create single entry within the archive. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_3)(string, string, bool, SevenZipEntrySettings) | Create single entry within the archive. |
| [Dispose](../../aspose.zip.sevenzip/sevenziparchive/dispose/)() | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [ExtractToDirectory](../../aspose.zip.sevenzip/sevenziparchive/extracttodirectory/)(string, string) | Extracts all the files in the archive to the directory provided. |
| [Save](../../aspose.zip.sevenzip/sevenziparchive/save/#save)(Stream) | Saves 7z archive to the stream provided. |
| [Save](../../aspose.zip.sevenzip/sevenziparchive/save/#save_1)(string) | Saves archive to destination file provided. |
| [SaveSplit](../../aspose.zip.sevenzip/sevenziparchive/savesplit/)(string, SplitSevenZipArchiveSaveOptions) | Saves multi-volume archive to destination directory provided. |

### See Also

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.SevenZip](../../aspose.zip.sevenzip/)
* assembly [Aspose.Zip](../../)


