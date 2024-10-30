---
title: SevenZipArchive
second_title: Aspose.Zip for Python via .NET API Reference
description: 
type: docs
weight: 10
url: /python-net/aspose.zip.sevenzip/sevenziparchive/
---

## SevenZipArchive class

This class represents 7z archive file. Use it to compose and extract 7z archives.

The SevenZipArchive type exposes the following members:
## Constructors
| Name | Description |
| :- | :- |
|SevenZipArchive(new_entry_settings)|Initializes a new instance of the [SevenZipArchive](/zip/python-net/aspose.zip.sevenzip/sevenziparchive/) class with optional settings for its entries.|
|SevenZipArchive(source_stream, password)|Initializes a new instance of the [SevenZipArchive](/zip/python-net/aspose.zip.sevenzip/sevenziparchive/) class and composes entries list can be extracted from the archive.|
|SevenZipArchive(path, password)|Initializes a new instance of the [SevenZipArchive](/zip/python-net/aspose.zip.sevenzip/sevenziparchive/) class and composes entries list can be extracted from the archive.|
|SevenZipArchive(parts, password)|Initializes a new instance of the [SevenZipArchive](/zip/python-net/aspose.zip.sevenzip/sevenziparchive/) class from multi-volume 7z archive and composes entries list can be extracted from the archive.|
## Properties
| Name | Description |
| :- | :- |
|new_entry_settings|Compression and encryption settings used for newly added [SevenZipArchiveEntry](/zip/python-net/aspose.zip.sevenzip/sevenziparchiveentry/) items.|
|entries|Gets entries of [SevenZipArchiveEntry](/zip/python-net/aspose.zip.sevenzip/sevenziparchiveentry/) type constituting the archive.|
|file_entries|Gets entries of [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) type constituting the archive.|
## Methods
| Name | Description |
| :- | :- |
|create_entry(name, source, new_entry_settings)|Create single entry within the archive.|
|create_entry(name, path, open_immediately, new_entry_settings)|Create single entry within the archive.|
|save(output)|Saves 7z archive to the stream provided.|
|save(destination_file_name)|Saves archive to destination file provided.|
|extract_to_directory(destination_directory, password)|Extracts all the files in the archive to the directory provided.|
|extract_to_directory(destination_directory)|Extracts all the files in the archive to the directory provided.|
|create_entries(source_directory, include_root_directory)|Adds to the archive all files and directories recursively in the directory given.|
|save_split(destination_directory, options)|Saves multi-volume archive to destination directory provided.|

### See Also

* namespace [aspose.zip.sevenzip](/zip/python-net/aspose.zip.sevenzip/)
* assembly [Aspose.Zip](/zip/python-net/)

