---
title: LzipArchive
second_title: Aspose.Zip for Python via .NET API Reference
description: 
type: docs
weight: 10
url: /python-net/aspose.zip.lzip/lziparchive/
---

## LzipArchive class

This class represents a Lzip archive file. Use it to compose or extract Lzip archives.

The LzipArchive type exposes the following members:
## Constructors
| Name | Description |
| :- | :- |
|LzipArchive(settings)|Initializes a new instance of the [LzipArchive](/zip/python-net/aspose.zip.lzip/lziparchive/).|
|LzipArchive(source_stream)|Initializes a new instance of the [LzipArchive](/zip/python-net/aspose.zip.lzip/lziparchive/) class prepared for decompressing.|
|LzipArchive(path)|Initializes a new instance of the [LzipArchive](/zip/python-net/aspose.zip.lzip/lziparchive/) class prepared for decompressing.|
## Properties
| Name | Description |
| :- | :- |
|settings|Gets the setting of particular lzip archive.|
|file_entries|Gets entries of [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) type constituting the archive.|
|format|Gets the archive format.|
|name|Gets name of the entry.|
|length|Gets the length of the entry in bytes.|
## Methods
| Name | Description |
| :- | :- |
|extract(destination)|Extracts lzip archive to a stream.|
|extract(path)|Extracts lzip archive to a file by path.|
|save(output_stream)|Saves lzip archive to the stream provided.|
|save(destination_file_name)|Saves lzip archive to destination file provided.|
|set_source(source)|Sets the content to be compressed within the archive.|
|set_source(path)|Sets the content to be compressed within the archive.|
|extract_to_directory(destination_directory)|Extracts content of the archive to the directory provided.|

### See Also

* namespace [aspose.zip.lzip](/zip/python-net/aspose.zip.lzip/)
* assembly [Aspose.Zip](/zip/python-net/)

