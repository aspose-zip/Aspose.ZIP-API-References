---
title: ArchiveEntry
second_title: Aspose.Zip for Python via .NET API Reference
description: 
type: docs
weight: 80
url: /python-net/aspose.zip/archiveentry/
---

## ArchiveEntry class

Represents single file within archive.

The ArchiveEntry type exposes the following members:
## Properties
| Name | Description |
| :- | :- |
|compressed_size|Gets size of compressed file.|
|name|Gets name of the entry within archive.|
|comment|Gets comment of the entry within archive.|
|uncompressed_size|Gets size of original file.|
|modification_time|Gets or sets last modified date and time.|
|is_directory|Gets a value indicating whether the entry represents directory.|
|compression_settings|Gets settings for compression or decompression.|
|length|Gets the length of the entry in bytes.|
## Methods
| Name | Description |
| :- | :- |
|extract(path, password)|Extracts the entry to the filesystem by the path provided.|
|extract(destination, password)|Extracts the entry to the stream provided.|
|extract(path)|Extracts the entry to the filesystem by the path provided.|
|extract(destination)|Extracts the entry to the stream provided.|
|open(password)|Opens the entry for extraction and provides a stream with decompressed entry content.|

### See Also

* namespace [aspose.zip](/zip/python-net/aspose.zip/)
* assembly [Aspose.Zip](/zip/python-net/)

