---
title: SevenZipArchiveEntry
second_title: Aspose.Zip for Python via .NET API Reference
description: 
type: docs
weight: 20
url: /python-net/aspose.zip.sevenzip/sevenziparchiveentry/
---

## SevenZipArchiveEntry class

Represents a single file within 7z archive.

The SevenZipArchiveEntry type exposes the following members:
## Properties
| Name | Description |
| :- | :- |
|name|Gets name of the entry within the archive.|
|modification_time|Gets last modified date and time.|
|uncompressed_size|Gets size of an original file.|
|compressed_size|Gets the size of a compressed file.|
|is_directory|Gets a value indicating whether the entry represents a directory.|
|compression_settings|Gets settings for compression or decompression.|
|length|Gets the length of the entry in bytes.|
## Methods
| Name | Description |
| :- | :- |
|extract(path, password)|Extracts the entry to the filesystem by the path provided.|
|extract(destination, password)|Extracts the entry to the stream provided.|
|extract(path)|Extracts the entry to the filesystem by the path provided.|
|extract(destination)|Extracts the entry to the stream provided.|
|open(password)|Opens the entry for extraction and provides a stream with entry content.|

### See Also

* namespace [aspose.zip.sevenzip](/zip/python-net/aspose.zip.sevenzip/)
* assembly [Aspose.Zip](/zip/python-net/)

