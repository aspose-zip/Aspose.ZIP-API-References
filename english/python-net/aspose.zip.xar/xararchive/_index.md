---
title: XarArchive
second_title: Aspose.Zip for Python via .NET API Reference
description: 
type: docs
weight: 10
url: /python-net/aspose.zip.xar/xararchive/
---

## XarArchive class

This class represents xar archive file.

The XarArchive type exposes the following members:
## Constructors
| Name | Description |
| :- | :- |
|XarArchive(default_compression_settings)|Initializes a new instance of the XarArchive class|
|XarArchive(source_stream)|Initializes a new instance of the XarArchive class|
|XarArchive(path)|Initializes a new instance of the XarArchive class|
## Properties
| Name | Description |
| :- | :- |
|entries|Gets entries of|
|file_entries|Gets entries of|
## Methods
| Name | Description |
| :- | :- |
|create_entry(name, source_path, open_immediately, compression_settings)|Create single entry within the archive.|
|create_entry(name, source, compression_settings)|Create single entry within the archive.|
|save(destination_file_name)|Saves archive to destination file provided.|
|save(output)|Saves archive to the stream provided.|
|extract_to_directory(destination_directory)|Extracts all the files in the archive to the directory provided.|
|create_entries(source_directory, include_root_directory, compression_settings)|Adds to the archive all the files and directories recursively in the directory given.|
|delete_entry(entry)|Removes the first occurrence of a specific entry from the entries list.|

### See Also

* namespace [aspose.zip.xar](/zip/python-net/aspose.zip.xar/)
* assembly [Aspose.Zip](/zip/python-net/)

