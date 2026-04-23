---
title: AppleArchive
second_title: Aspose.Zip for Python via .NET API Reference
description: 
type: docs
weight: 10
url: /python-net/aspose.zip.apple/applearchive/
---

## AppleArchive class

This class represents an Apple Archive (.aar) file. Use it to compose Apple Archive files.

The AppleArchive type exposes the following members:
## Constructors
| Name | Description |
| :- | :- |
|AppleArchive(new_entry_settings)|Initializes a new instance of the [AppleArchive](/zip/python-net/aspose.zip.apple/applearchive/) class with settings used for composed entries.|
## Properties
| Name | Description |
| :- | :- |
|entries|Gets entries constituting the archive.|
|new_entry_settings|Gets settings used for newly composed entries.|
|file_entries|Gets entries of [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) type constituting the archive.|
|format|Gets the archive format.|
## Methods
| Name | Description |
| :- | :- |
|create_entry(name, path, open_immediately)|Creates a single entry within the archive.|
|create_entry(name, source)|Creates a single entry within the archive.|
|save(output)|Saves archive to the stream provided.|
|save(destination_file_name)|Saves archive to a destination file provided.|
|extract_to_directory(destination_directory)|Extracts all the files in the archive to the directory provided.|

### See Also

* namespace [aspose.zip.apple](/zip/python-net/aspose.zip.apple/)
* assembly [Aspose.Zip](/zip/python-net/)

