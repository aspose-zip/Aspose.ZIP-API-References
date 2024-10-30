---
title: SharArchive
second_title: Aspose.Zip for Python via .NET API Reference
description: 
type: docs
weight: 10
url: /python-net/aspose.zip.shar/shararchive/
---

## SharArchive class

This class represents shar archive file.

The SharArchive type exposes the following members:
## Constructors
| Name | Description |
| :- | :- |
|SharArchive()|Initializes a new instance of the [SharArchive](/zip/python-net/aspose.zip.shar/shararchive/) class.|
|SharArchive(path)|Initializes a new instance of the [SharArchive](/zip/python-net/aspose.zip.shar/shararchive/) class prepared for decompressing.|
## Properties
| Name | Description |
| :- | :- |
|entries|Gets entries of [SharEntry](/zip/python-net/aspose.zip.shar/sharentry/) type constituting the archive.|
## Methods
| Name | Description |
| :- | :- |
|create_entry(name, source_path, open_immediately)|Create single entry within the archive.|
|create_entry(name, source)|Create single entry within the archive.|
|delete_entry(entry)|Removes the first occurrence of a specific entry from the entries list.|
|delete_entry(entry_index)|Removes the entry from the entries list by index.|
|save(destination_file_name)|Saves archive to destination file provided.|
|save(output)|Saves archive to the stream provided.|
|create_entries(source_directory, include_root_directory)|Adds to the archive all the files and directories recursively in the directory given.|

### See Also

* namespace [aspose.zip.shar](/zip/python-net/aspose.zip.shar/)
* assembly [Aspose.Zip](/zip/python-net/)

