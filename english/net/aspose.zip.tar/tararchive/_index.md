---
title: Class TarArchive
second_title: Aspose.ZIP for .NET API Reference
description: Aspose.Zip.Tar.TarArchive class. This class represents tar archive file. Use it to compose extract or update tar archives
type: docs
weight: 870
url: /net/aspose.zip.tar/tararchive/
---
## TarArchive class

This class represents tar archive file. Use it to compose, extract, or update tar archives.

```csharp
public class TarArchive : IArchive
```

## Constructors

| Name | Description |
| --- | --- |
| [TarArchive](tararchive/#constructor)() | Initializes a new instance of the `TarArchive` class. |
| [TarArchive](tararchive/#constructor_1)(Stream) | Initializes a new instance of the [`Archive`](../../aspose.zip/archive/) class and composes entry list can be extracted from the archive. |
| [TarArchive](tararchive/#constructor_2)(string) | Initializes a new instance of the `TarArchive` class and composes entries list can be extracted from the archive. |

## Properties

| Name | Description |
| --- | --- |
| [Entries](../../aspose.zip.tar/tararchive/entries/) { get; } | Gets entries of [`TarEntry`](../tarentry/) type constituting the archive. |

## Methods

| Name | Description |
| --- | --- |
| static [FromGZip](../../aspose.zip.tar/tararchive/fromgzip/#fromgzip)(Stream) | Extracts supplied gzip archive and composes `TarArchive` from extracted data. |
| static [FromGZip](../../aspose.zip.tar/tararchive/fromgzip/#fromgzip_1)(string) | Extracts supplied gzip archive and composes `TarArchive` from extracted data. |
| static [FromLZip](../../aspose.zip.tar/tararchive/fromlzip/#fromlzip)(Stream) | Extracts supplied lzip archive and composes `TarArchive` from extracted data. |
| static [FromLZip](../../aspose.zip.tar/tararchive/fromlzip/#fromlzip_1)(string) | Extracts supplied lzip archive and composes `TarArchive` from extracted data. |
| static [FromLZMA](../../aspose.zip.tar/tararchive/fromlzma/#fromlzma)(Stream) | Extracts supplied LZMA archive and composes `TarArchive` from extracted data. |
| static [FromLZMA](../../aspose.zip.tar/tararchive/fromlzma/#fromlzma_1)(string) | Extracts supplied LZMA archive and composes `TarArchive` from extracted data. |
| static [FromXz](../../aspose.zip.tar/tararchive/fromxz/#fromxz)(Stream) | Extracts supplied xz format archive and composes `TarArchive` from extracted data. |
| static [FromXz](../../aspose.zip.tar/tararchive/fromxz/#fromxz_1)(string) | Extracts supplied xz format archive and composes `TarArchive` from extracted data. |
| static [FromZ](../../aspose.zip.tar/tararchive/fromz/#fromz)(Stream) | Extracts supplied Z format archive and composes `TarArchive` from extracted data. |
| static [FromZ](../../aspose.zip.tar/tararchive/fromz/#fromz_1)(string) | Extracts supplied Z format archive and composes `TarArchive` from extracted data. |
| static [FromZstandard](../../aspose.zip.tar/tararchive/fromzstandard/#fromzstandard)(Stream) | Extracts supplied Zstandard archive and composes `TarArchive` from extracted data. |
| static [FromZstandard](../../aspose.zip.tar/tararchive/fromzstandard/#fromzstandard_1)(string) | Extracts supplied Zstandard archive and composes `TarArchive` from extracted data. |
| [CreateEntries](../../aspose.zip.tar/tararchive/createentries/#createentries)(DirectoryInfo, bool) | Adds to the archive all the files and directories recursively in the directory given. |
| [CreateEntries](../../aspose.zip.tar/tararchive/createentries/#createentries_1)(string, bool) | Adds to the archive all the files and directories recursively in the directory given. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry/#createentry)(string, FileInfo, bool) | Create a single entry within the archive. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry/#createentry_1)(string, Stream, FileSystemInfo) | Create a single entry within the archive. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry/#createentry_2)(string, string, bool) | Create a single entry within the archive. |
| [DeleteEntry](../../aspose.zip.tar/tararchive/deleteentry/#deleteentry_1)(int) | Removes the entry from the entry list by index. |
| [DeleteEntry](../../aspose.zip.tar/tararchive/deleteentry/#deleteentry)(TarEntry) | Removes the first occurrence of a specific entry from the entry list. |
| [Dispose](../../aspose.zip.tar/tararchive/dispose/)() | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [ExtractToDirectory](../../aspose.zip.tar/tararchive/extracttodirectory/)(string) | Extracts all the files in the archive to the directory provided. |
| [Save](../../aspose.zip.tar/tararchive/save/#save)(Stream, TarFormat?) | Saves archive to the stream provided. |
| [Save](../../aspose.zip.tar/tararchive/save/#save_1)(string, TarFormat?) | Saves archive to a destination file provided. |
| [SaveGzipped](../../aspose.zip.tar/tararchive/savegzipped/#savegzipped)(Stream, TarFormat?) | Saves archive to the stream with gzip compression. |
| [SaveGzipped](../../aspose.zip.tar/tararchive/savegzipped/#savegzipped_1)(string, TarFormat?) | Saves archive to the file by path with gzip compression. |
| [SaveLzipped](../../aspose.zip.tar/tararchive/savelzipped/#savelzipped)(Stream, TarFormat?) | Saves archive to the stream with lzip compression. |
| [SaveLzipped](../../aspose.zip.tar/tararchive/savelzipped/#savelzipped_1)(string, TarFormat?) | Saves archive to the file by path with lzip compression. |
| [SaveLZMACompressed](../../aspose.zip.tar/tararchive/savelzmacompressed/#savelzmacompressed)(Stream, TarFormat?) | Saves archive to the stream with LZMA compression. |
| [SaveLZMACompressed](../../aspose.zip.tar/tararchive/savelzmacompressed/#savelzmacompressed_1)(string, TarFormat?) | Saves archive to the file by path with lzma compression. |
| [SaveXzCompressed](../../aspose.zip.tar/tararchive/savexzcompressed/#savexzcompressed)(Stream, TarFormat?, XzArchiveSettings) | Saves archive to the stream with xz compression. |
| [SaveXzCompressed](../../aspose.zip.tar/tararchive/savexzcompressed/#savexzcompressed_1)(string, TarFormat?, XzArchiveSettings) | Saves archive to the path by path with xz compression. |
| [SaveZCompressed](../../aspose.zip.tar/tararchive/savezcompressed/#savezcompressed)(Stream, TarFormat?) | Saves archive to the stream with Z compression. |
| [SaveZCompressed](../../aspose.zip.tar/tararchive/savezcompressed/#savezcompressed_1)(string, TarFormat?) | Saves archive to the path by path with Z compression. |
| [SaveZstandard](../../aspose.zip.tar/tararchive/savezstandard/#savezstandard)(Stream, TarFormat?) | Saves archive to the stream with Zstandard compression. |
| [SaveZstandard](../../aspose.zip.tar/tararchive/savezstandard/#savezstandard_1)(string, TarFormat?) | Saves archive to the file by path with Zstandard compression. |

### See Also

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Tar](../../aspose.zip.tar/)
* assembly [Aspose.Zip](../../)


