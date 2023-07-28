---
title: CpioArchive
second_title: Aspose.Sildes for Python via .NET API Reference
description: 
type: docs
weight: 10
url: /python-net/aspose.zip.cpio/cpioarchive/
---

## CpioArchive class

This class represents cpio archive file.

The CpioArchive type exposes the following members:
## Constructors
| Name | Description |
| :- | :- |
|CpioArchive()|Initializes a new instance of the [CpioArchive](/zip/python-net/aspose.zip.cpio/cpioarchive/) class.|
|CpioArchive(source_stream)|Initializes a new instance of the CpioArchive class|
|CpioArchive(path)|Initializes a new instance of the CpioArchive class|
## Properties
| Name | Description |
| :- | :- |
|entries|Gets entries of|
|file_entries|Gets entries of|
## Methods
| Name | Description |
| :- | :- |
|create_entry(name, source_path, open_immediately)|Create single entry within the archive.|
|create_entry(name, source)|Create single entry within the archive.|
|delete_entry(entry)|Removes the first occurrence of a specific entry from the entries list.|
|delete_entry(entry_index)|Removes the entry from the entries list by index.|
|save(destination_file_name, cpio_format)|Saves archive to destination file provided.|
|save(output, cpio_format)|Saves archive to the stream provided.|
|save_gzipped(output, cpio_format)|Saves archive to the stream with gzip compression.|
|save_gzipped(path, cpio_format)|Saves archive to the file by path with gzip compression.|
|save_xz_compressed(output, cpio_format, settings)|Saves archive to the stream with xz compression.|
|save_xz_compressed(path, cpio_format, settings)|Saves archive to the path by path with xz compression.|
|create_entries(source_directory, include_root_directory)|Adds to the archive all the files and directories recursively in the directory given.|
|extract_to_directory(destination_directory)|Extracts all the files in the archive to the directory provided.|

### See Also

* namespace [aspose.zip.cpio](/zip/python-net/aspose.zip.cpio/)
* assembly [Aspose.Zip](/zip/python-net/)

