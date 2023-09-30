---
title: Archive
second_title: Aspose.Zip for Python via .NET API Reference
description: 
type: docs
weight: 10
url: /python-net/aspose.zip/archive/
---

## Archive class

This class represents zip archive file. Use it to compose, extract, or update zip archives.

The Archive type exposes the following members:
## Constructors
| Name | Description |
| :- | :- |
|Archive(new_entry_settings)|Initializes a new instance of the Archive class|
|Archive(source_stream, load_options, new_entry_settings)|Initializes a new instance of the Archive class|
|Archive(path, load_options, new_entry_settings)|Initializes a new instance of the Archive class|
## Properties
| Name | Description |
| :- | :- |
|new_entry_settings|Compression and encryption settings used for newly added|
|entries|Gets entries of|
|file_entries|Gets entries of|
## Methods
| Name | Description |
| :- | :- |
|create_entry(name, path, open_immediately, new_entry_settings)|Create single entry within the archive.|
|create_entry(name, source, new_entry_settings)|Create single entry within the archive.|
|delete_entry(entry)|Removes the first occurrence of a specific entry from the entries list.|
|delete_entry(entry_index)|Removes the entry from the entries list by index.|
|save(output_stream, save_options)|Saves archive to the stream provided.|
|save(destination_file_name, save_options)|Saves archive to destination file provided.|
|create_entries(source_directory, include_root_directory)|Adds to the archive all files and directories recursively in the directory given.|
|save_split(destination_directory, options)|Saves multi-volume archive to destination directory provided.|
|extract_to_directory(destination_directory)|Extracts all the files in the archive to the directory provided.|

### See Also

* namespace [aspose.zip](/zip/python-net/aspose.zip/)
* assembly [Aspose.Zip](/zip/python-net/)

