---
title: RarArchiveEntryEncrypted
second_title: Aspose.Zip for Python via .NET API Reference
description: 
type: docs
weight: 30
url: /python-net/aspose.zip.rar/rararchiveentryencrypted/
---

## RarArchiveEntryEncrypted class

Zip entry that needs to be decompressed with decryption.

The RarArchiveEntryEncrypted type exposes the following members:
## Properties
| Name | Description |
| :- | :- |
|name|Gets name of the entry within archive.|
|compressed_size|Gets size of compressed file.|
|uncompressed_size|Gets size of original file.|
|modification_time|Gets last modified date and time.|
|creation_time|Gets creation date and time.|
|last_access_time|Gets last access date and time.|
|is_directory|Gets a value indicating whether the entry represents directory.|
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

* namespace [aspose.zip.rar](/zip/python-net/aspose.zip.rar/)
* assembly [Aspose.Zip](/zip/python-net/)

