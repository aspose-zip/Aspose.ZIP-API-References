---
title: IsoArchive
second_title: Aspose.Zip for Python via .NET API Reference
description: 
type: docs
weight: 30
url: /python-net/aspose.zip.iso/isoarchive/
---

## IsoArchive class

Represents an ISO archive (ISO 9660).

The IsoArchive type exposes the following members:
## Constructors
| Name | Description |
| :- | :- |
|IsoArchive()|Initializes a new instance of the [IsoArchive](/zip/python-net/aspose.zip.iso/isoarchive/) class and creates an empty ISO archive<br/>             for adding new files and directories.|
|IsoArchive(source_stream, load_options)|Initializes a new instance of the [IsoArchive](/zip/python-net/aspose.zip.iso/isoarchive/) class and composes an entry list that can be extracted from the archive.|
|IsoArchive(path, load_options)|Initializes a new instance of the [IsoArchive](/zip/python-net/aspose.zip.iso/isoarchive/) class and composes an entry list that can be extracted from the archive.|
## Properties
| Name | Description |
| :- | :- |
|entries|Gets entries of [IsoEntry](/zip/python-net/aspose.zip.iso/isoentry/) type constituting the archive.|
|file_entries|Gets entries of [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) type constituting the archive.|
|format|Gets the archive format.|
## Methods
| Name | Description |
| :- | :- |
|create_entry(name, file_path)|Adds a file to the ISO image.|
|create_entry(name, source)|Adds a file to the ISO image.|
|create_entry(name)|Adds a file to the ISO image.|
|save(path, save_options)|Saves the ISO image to the specified path.|
|save(stream, save_options)|Saves the ISO image to the specified stream.|
|create_directory(name)|Adds a directory to the ISO image.|
|extract_to_directory(destination_directory)|Extracts all entries to the specified directory.|

### See Also

* namespace [aspose.zip.iso](/zip/python-net/aspose.zip.iso/)
* assembly [Aspose.Zip](/zip/python-net/)

