---
title: Lz4Archive
second_title: Aspose.Zip for Python via .NET API Reference
description: 
type: docs
weight: 10
url: /python-net/aspose.zip.lz4/lz4archive/
---

## Lz4Archive class

This class represents LZ4 archive file. Use it to extract or compose LZ4 archives.

The Lz4Archive type exposes the following members:
## Constructors
| Name | Description |
| :- | :- |
|Lz4Archive(source_stream, load_options)|Initializes a new instance of the [Lz4Archive](/zip/python-net/aspose.zip.lz4/lz4archive/) class prepared for decompressing.|
|Lz4Archive(path, load_options)|Initializes a new instance of the [Lz4Archive](/zip/python-net/aspose.zip.lz4/lz4archive/) class.|
|Lz4Archive(settings)|Initializes a new instance of the [Lz4Archive](/zip/python-net/aspose.zip.lz4/lz4archive/) class prepared for compressing.|
## Properties
| Name | Description |
| :- | :- |
|file_entries|Gets entries of [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) type constituting the archive.|
|format|Gets the archive format.|
|name|Gets name of the entry.|
|length|Gets the length of the entry in bytes.|
## Methods
| Name | Description |
| :- | :- |
|extract(path)|Extracts the archive to the file by path.|
|extract(destination)|Extracts the archive to the stream provided.|
|save(output)|Saves lz4 archive to the stream provided.|
|save(destination_file_name)|Saves archive to the destination file provided.|
|set_source(source)|Sets the content to be compressed within the archive.|
|set_source(tar_archive, format)|Sets the content to be compressed within the archive.|
|set_source(path)|Sets the content to be compressed within the archive.|
|extract_to_directory(destination_directory)|Extracts content of the archive to the directory provided.|
|open()|Opens the archive for extraction and provides a stream with archive content.|

### See Also

* namespace [aspose.zip.lz4](/zip/python-net/aspose.zip.lz4/)
* assembly [Aspose.Zip](/zip/python-net/)

