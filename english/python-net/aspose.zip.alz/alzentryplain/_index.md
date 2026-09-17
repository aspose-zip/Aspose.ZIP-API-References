---
title: AlzEntryPlain
second_title: Aspose.Zip for Python via .NET API Reference
description: 
type: docs
weight: 50
url: /python-net/aspose.zip.alz/alzentryplain/
---

## AlzEntryPlain class

ALZ entry that needs to be decompressed without decryption.

The AlzEntryPlain type exposes the following members:
## Properties
| Name | Description |
| :- | :- |
|compressed_size|Compressed size of the file data in bytes.|
|uncompressed_size|Uncompressed size of the file data in bytes.|
|length|Gets the length of the entry in bytes.|
|is_directory|Returns true if this entry represents a directory.|
|name|File name (without path).|
## Methods
| Name | Description |
| :- | :- |
|extract(path, password)|Extracts the entry to the filesystem by the path provided.|
|extract(destination, password)|Extracts the entry to the stream provided.|
|extract(path)|Extracts the entry to the filesystem by the path provided.|
|extract(destination)|Extracts the entry to the stream provided.|
|open(password)|Opens the entry for extraction and provides a stream with decompressed entry content.|

### See Also

* namespace [aspose.zip.alz](/zip/python-net/aspose.zip.alz/)
* assembly [Aspose.Zip](/zip/python-net/)

