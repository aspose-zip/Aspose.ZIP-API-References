---
title: WimArchive
second_title: Aspose.Zip for Python via .NET API Reference
description: 
type: docs
weight: 10
url: /python-net/aspose.zip.wim/wimarchive/
---

## WimArchive class

This class represents wim archive file.

The WimArchive type exposes the following members:
## Constructors
| Name | Description |
| :- | :- |
|WimArchive(source_stream)|Initializes a new instance of the [WimArchive](/zip/python-net/aspose.zip.wim/wimarchive/) class and composes entries list can be extracted from the archive.|
|WimArchive(path)|Initializes a new instance of the [WimArchive](/zip/python-net/aspose.zip.wim/wimarchive/) class and composes entries list can be extracted from the archive.|
## Properties
| Name | Description |
| :- | :- |
|images|Gets entries of [WimImage](/zip/python-net/aspose.zip.wim/wimimage/) type constituting the archive.|
|guid|Gets the identifying GUID for the archive.|
|boot_image_index|Gets the (zero-based) index of the bootable image.|
|file_format_version|Gets the version of the file format.|
|manifest|Gets the embedded manifest describing the file and the contained images.|
|file_entries|Gets entries of [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) type constituting the archive.|
## Methods
| Name | Description |
| :- | :- |
|extract_to_directory(destination_directory)|Extracts the archive to the file by path.|

### See Also

* namespace [aspose.zip.wim](/zip/python-net/aspose.zip.wim/)
* assembly [Aspose.Zip](/zip/python-net/)

