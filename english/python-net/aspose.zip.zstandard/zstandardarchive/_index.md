---
title: ZstandardArchive
second_title: Aspose.Zip for Python via .NET API Reference
description: 
type: docs
weight: 10
url: /python-net/aspose.zip.zstandard/zstandardarchive/
---

## ZstandardArchive class

This class represents Zstandard archive file. Use it to compose Zstandard archives.

The ZstandardArchive type exposes the following members:
## Constructors
| Name | Description |
| :- | :- |
|ZstandardArchive()|Initializes a new instance of the [ZstandardArchive](/zip/python-net/aspose.zip.zstandard/zstandardarchive/) class prepared for compressing.|
|ZstandardArchive(source_stream, options)|Initializes a new instance of the ZstandardArchive class|
|ZstandardArchive(path, options)|Initializes a new instance of the ZstandardArchive class|
## Properties
| Name | Description |
| :- | :- |
|file_entries|Gets entries of|
|name|Gets name of the entry.|
|length|Gets the length of the entry in bytes.|
## Methods
| Name | Description |
| :- | :- |
|extract(destination)|Extracts the archive to the stream provided.|
|extract(path)|Extracts the archive to the file by path.|
|set_source(source)|Sets the content to be compressed within the archive.|
|set_source(path)|Sets the content to be compressed within the archive.|
|save(output_stream, settings)|Saves archive to the stream provided.|
|save(destination_file_name, settings)|Saves archive to destination file provided.|
|open()|Opens the archive for extraction and provides a stream with archive content.|
|extract_to_directory(destination_directory)|Extracts content of the archive to the directory provided.|

### See Also

* namespace [aspose.zip.zstandard](/zip/python-net/aspose.zip.zstandard/)
* assembly [Aspose.Zip](/zip/python-net/)

