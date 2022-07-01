---
title: TarArchive
second_title: Aspose.ZIP for .NET API Reference
description: 
type: docs
weight: 580
url: /net/aspose.zip.tar/tararchive/
---
## TarArchive class

This class represents tar archive file. Use it to compose, extract, or update tar archives.

```csharp
public class TarArchive : IDisposable
```

## Constructors

| Name | Description |
| --- | --- |
| [TarArchive](tararchive)() | Initializes a new instance of the [`TarArchive`](../tararchive) class. |
| [TarArchive](tararchive)(Stream) | Initializes a new instance of the [`Archive`](../../aspose.zip/archive) class and composes entries list can be extracted from the archive. |
| [TarArchive](tararchive)(string) | Initializes a new instance of the [`TarArchive`](../tararchive) class and composes entries list can be extracted from the archive. |

## Properties

| Name | Description |
| --- | --- |
| [Entries](../../aspose.zip.tar/tararchive/entries) { get; } | Gets entries of [`TarEntry`](../tarentry) type constituting the archive. |

## Methods

| Name | Description |
| --- | --- |
| static [FromGZip](../../aspose.zip.tar/tararchive/fromgzip)(Stream) | Extracts supplied gzip archive and composes [`TarArchive`](../tararchive) from extracted data. |
| static [FromGZip](../../aspose.zip.tar/tararchive/fromgzip)(string) | Extracts supplied gzip archive and composes [`TarArchive`](../tararchive) from extracted data. |
| static [FromLZip](../../aspose.zip.tar/tararchive/fromlzip)(Stream) | Extracts supplied lzip archive and composes [`TarArchive`](../tararchive) from extracted data. |
| static [FromLZip](../../aspose.zip.tar/tararchive/fromlzip)(string) | Extracts supplied lzip archive and composes [`TarArchive`](../tararchive) from extracted data. |
| static [FromXz](../../aspose.zip.tar/tararchive/fromxz)(Stream) | Extracts supplied xz format archive and composes [`TarArchive`](../tararchive) from extracted data. |
| static [FromXz](../../aspose.zip.tar/tararchive/fromxz)(string) | Extracts supplied xz format archive and composes [`TarArchive`](../tararchive) from extracted data. |
| static [FromZ](../../aspose.zip.tar/tararchive/fromz)(Stream) | Extracts supplied Z format archive and composes [`TarArchive`](../tararchive) from extracted data. |
| static [FromZ](../../aspose.zip.tar/tararchive/fromz)(string) | Extracts supplied Z format archive and composes [`TarArchive`](../tararchive) from extracted data. |
| [CreateEntries](../../aspose.zip.tar/tararchive/createentries)(DirectoryInfo, bool) | Adds to the archive all the files and directories recursively in the directory given. |
| [CreateEntries](../../aspose.zip.tar/tararchive/createentries)(string, bool) | Adds to the archive all the files and directories recursively in the directory given. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry)(string, FileInfo, bool) | Create single entry within the archive. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry)(string, Stream, FileSystemInfo) | Create single entry within the archive. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry)(string, string, bool) | Create single entry within the archive. |
| [DeleteEntry](../../aspose.zip.tar/tararchive/deleteentry)(int) | Removes the entry from the entries list by index. |
| [DeleteEntry](../../aspose.zip.tar/tararchive/deleteentry)(TarEntry) | Removes the first occurrence of a specific entry from the entries list. |
| [Dispose](../../aspose.zip.tar/tararchive/dispose)() | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [ExtractToDirectory](../../aspose.zip.tar/tararchive/extracttodirectory)(string) | Extracts all the files in the archive to the directory provided. |
| [Save](../../aspose.zip.tar/tararchive/save)(Stream, TarFormat?) | Saves archive to the stream provided. |
| [Save](../../aspose.zip.tar/tararchive/save)(string, TarFormat?) | Saves archive to destination file provided. |
| [SaveGzipped](../../aspose.zip.tar/tararchive/savegzipped)(Stream, TarFormat?) | Saves archive to the stream with gzip compression. |
| [SaveGzipped](../../aspose.zip.tar/tararchive/savegzipped)(string, TarFormat?) | Saves archive to the file by path with gzip compression. |
| [SaveLzipped](../../aspose.zip.tar/tararchive/savelzipped)(Stream, TarFormat?) | Saves archive to the stream with lzip compression. |
| [SaveLzipped](../../aspose.zip.tar/tararchive/savelzipped)(string, TarFormat?) | Saves archive to the file by path with lzip compression. |
| [SaveXzCompressed](../../aspose.zip.tar/tararchive/savexzcompressed)(Stream, TarFormat?, XzArchiveSettings) | Saves archive to the stream with xz compression. |
| [SaveXzCompressed](../../aspose.zip.tar/tararchive/savexzcompressed)(string, TarFormat?, XzArchiveSettings) | Saves archive to the path by path with xz compression. |
| [SaveZCompressed](../../aspose.zip.tar/tararchive/savezcompressed)(Stream, TarFormat?) | Saves archive to the stream with Z compression. |
| [SaveZCompressed](../../aspose.zip.tar/tararchive/savezcompressed)(string, TarFormat?) | Saves archive to the path by path with Z compression. |

### See Also

* namespace [Aspose.Zip.Tar](../../aspose.zip.tar)
* assembly [Aspose.Zip](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.ZIP.dll -->
