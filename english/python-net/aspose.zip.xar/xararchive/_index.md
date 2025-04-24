---
title: XarArchive
second_title: Aspose.Zip for Python via .NET API Reference
description: 
type: docs
weight: 80
url: /python-net/aspose.zip.xar/xararchive/
---

## XarArchive class

This class represents a xar archive file.

The XarArchive type exposes the following members:
## Constructors
| Name | Description |
| :- | :- |
|XarArchive(default_compression_settings)|Initializes a new instance of the [XarArchive](/zip/python-net/aspose.zip.xar/xararchive/) class.|
|XarArchive(source_stream, load_options)|Initializes a new instance of the [XarArchive](/zip/python-net/aspose.zip.xar/xararchive/) class and composes an entry list can be extracted from the archive.|
|XarArchive(path, load_options)|Initializes a new instance of the [XarArchive](/zip/python-net/aspose.zip.xar/xararchive/) class and composes an entry list can be extracted from the archive.|
## Properties
| Name | Description |
| :- | :- |
|entries|Gets entries of [XarEntry](/zip/python-net/aspose.zip.xar/xarentry/) type constituting the archive.|
|file_entries|Gets entries of [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) type constituting the archive.|
|format|Gets the archive format.|
## Methods
| Name | Description |
| :- | :- |
|create_entry(name, source_path, open_immediately, compression_settings)|Create a single entry within the archive.|
|create_entry(name, source, compression_settings)|Create a single entry within the archive.|
|save(destination_file_name, save_options)|Saves archive to the destination file provided.|
|save(output, save_options)|Saves archive to the stream provided.|
|extract_to_directory(destination_directory)|Extracts all the files in the archive to the directory provided.|
|create_entries(source_directory, include_root_directory, compression_settings)|Adds to the archive all the files and directories recursively in the directory given.|
|delete_entry(entry)|Removes the first occurrence of a specific entry from the entry list.|

### See Also

* namespace [aspose.zip.xar](/zip/python-net/aspose.zip.xar/)
* assembly [Aspose.Zip](/zip/python-net/)

