---
title: XzArchive
second_title: Aspose.Zip for Python via .NET API Reference
description: 
type: docs
weight: 10
url: /python-net/aspose.zip.xz/xzarchive/
---

## XzArchive class

This class represents xz archive file. Use it to compose and extract xz archives.

The XzArchive type exposes the following members:
## Constructors
| Name | Description |
| :- | :- |
|XzArchive(settings)|Initializes a new instance of the [XzArchive](/zip/python-net/aspose.zip.xz/xzarchive/) class and composes the archive in xz format.|
|XzArchive(source)|Initializes a new instance of the [XzArchive](/zip/python-net/aspose.zip.xz/xzarchive/) class prepared for decompressing.|
|XzArchive(path)|Initializes a new instance of the [XzArchive](/zip/python-net/aspose.zip.xz/xzarchive/) class prepared for decompressing.|
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
|extract(destination)|Extracts xz archive to a stream.|
|extract(path)|Extracts content of the archive to the directory provided.|
|set_source(source)|Sets the content to be compressed within the archive.|
|set_source(source_path)|Sets the content to be compressed within the archive.|
|save(output)|Saves xz archive to the stream provided.|
|save(destination_file_name)|Saves xz archive to destination file provided.|
|extract_to_directory(destination_directory)|Extracts content of the archive to the directory provided.|

### See Also

* namespace [aspose.zip.xz](/zip/python-net/aspose.zip.xz/)
* assembly [Aspose.Zip](/zip/python-net/)

