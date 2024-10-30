---
title: LzmaArchive
second_title: Aspose.Zip for Python via .NET API Reference
description: 
type: docs
weight: 10
url: /python-net/aspose.zip.lzma/lzmaarchive/
---

## LzmaArchive class

This class represents LZMA archive file. Use it to compose or extract LZMA archives.

The LzmaArchive type exposes the following members:
## Constructors
| Name | Description |
| :- | :- |
|LzmaArchive(settings)|Initializes a new instance of the [LzmaArchive](/zip/python-net/aspose.zip.lzma/lzmaarchive/) class and composes the archive in lzma format.|
|LzmaArchive(source)|Initializes a new instance of the [LzmaArchive](/zip/python-net/aspose.zip.lzma/lzmaarchive/) class prepared for decompressing.|
|LzmaArchive(path)|Initializes a new instance of the [LzmaArchive](/zip/python-net/aspose.zip.lzma/lzmaarchive/) class prepared for decompressing.|
## Properties
| Name | Description |
| :- | :- |
|file_entries|Gets entries of [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) type constituting the archive.|
|name|Gets name of the entry.|
|length|Gets the length of the entry in bytes.|
## Methods
| Name | Description |
| :- | :- |
|extract(destination)|Extracts lzma archive to a stream.|
|extract(path)|Extracts lzma archive to a file by path.|
|set_source(source)|Sets the content to be compressed within the archive.|
|set_source(source_path)|Sets the content to be compressed within the archive.|
|save(output)|Saves lzma archive to the stream provided.|
|save(destination_file_name)|Saves lzma archive to destination file provided.|
|extract_to_directory(destination_directory)|Extracts content of the archive to the directory provided.|

### See Also

* namespace [aspose.zip.lzma](/zip/python-net/aspose.zip.lzma/)
* assembly [Aspose.Zip](/zip/python-net/)

