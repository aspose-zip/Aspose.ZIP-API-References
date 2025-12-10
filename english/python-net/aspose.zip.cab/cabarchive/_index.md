---
title: CabArchive
second_title: Aspose.Zip for Python via .NET API Reference
description: 
type: docs
weight: 10
url: /python-net/aspose.zip.cab/cabarchive/
---

## CabArchive class

This class represents a CAB archive file.

The CabArchive type exposes the following members:
## Constructors
| Name | Description |
| :- | :- |
|CabArchive(settings)|Initializes a new instance of the [CabArchive](/zip/python-net/aspose.zip.cab/cabarchive/) class prepared for compressing.|
|CabArchive(source_stream, load_options)|Initializes a new instance of the [CabArchive](/zip/python-net/aspose.zip.cab/cabarchive/) class and composes an entry list can be extracted from the archive.|
|CabArchive(path, load_options)|Initializes a new instance of the [CabArchive](/zip/python-net/aspose.zip.cab/cabarchive/) class and composes an entry list can be extracted from the archive.|
## Properties
| Name | Description |
| :- | :- |
|entries|Gets entries of [CabEntry](/zip/python-net/aspose.zip.cab/cabentry/) type constituting the archive.|
|file_entries|Gets entries of [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) type constituting the archive.|
|format|Gets the archive format.|
## Methods
| Name | Description |
| :- | :- |
|create_entry(name, path, new_entry_settings)|Create a single entry within the archive.|
|create_entry(name, source, new_entry_settings)|Create a single entry within the archive.|
|save(output_stream, save_options)|Saves archive to the stream provided.|
|save(destination_file_name, save_options)|Saves archive to the destination file provided.|
|create_entries(source_directory, include_root_directory)|Adds to the archive all files recursively from the specified directory path.|
|extract_to_directory(destination_directory)|Extracts all the files in the archive to the directory provided.|

### See Also

* namespace [aspose.zip.cab](/zip/python-net/aspose.zip.cab/)
* assembly [Aspose.Zip](/zip/python-net/)

