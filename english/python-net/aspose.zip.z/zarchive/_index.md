---
title: ZArchive
second_title: Aspose.Zip for Python via .NET API Reference
description: 
type: docs
weight: 10
url: /python-net/aspose.zip.z/zarchive/
---

## ZArchive class

This class represents Z (compress) archive file. Use it to compose or extract Z archives.

The ZArchive type exposes the following members:
## Constructors
| Name | Description |
| :- | :- |
|ZArchive()|Initializes a new instance of the [ZArchive](/zip/python-net/aspose.zip.z/zarchive/) class prepared for compressing.|
|ZArchive(source, load_options)|Initializes a new instance of the ZArchive class|
|ZArchive(path, load_options)|Initializes a new instance of the ZArchive class|
## Properties
| Name | Description |
| :- | :- |
|file_entries|Gets entries of [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) type constituting the archive.|
|name|Gets name of the entry.|
|length|Gets the length of the entry in bytes.|
## Methods
| Name | Description |
| :- | :- |
|extract(destination)|Extracts Z archive to a stream.|
|extract(path)|Extracts Z archive to a file by path.|
|save(output, settings)|Saves xz archive to the stream provided.|
|save(destination_file_name, settings)|Saves Z archive to destination file provided.|
|set_source(source)|Sets the content to be compressed within the archive.|
|set_source(source_path)|Sets the content to be compressed within the archive.|
|extract_to_directory(destination_directory)|Extracts content of the archive to the directory provided.|

### See Also

* namespace [aspose.zip.z](/zip/python-net/aspose.zip.z/)
* assembly [Aspose.Zip](/zip/python-net/)

