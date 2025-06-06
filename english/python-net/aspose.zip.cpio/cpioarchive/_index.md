---
title: CpioArchive
second_title: Aspose.Zip for Python via .NET API Reference
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
|CpioArchive(source_stream)|Initializes a new instance of the [CpioArchive](/zip/python-net/aspose.zip.cpio/cpioarchive/) class and composes an entry list can be extracted from the archive.|
|CpioArchive(path)|Initializes a new instance of the [CpioArchive](/zip/python-net/aspose.zip.cpio/cpioarchive/) class and composes an entry list can be extracted from the archive.|
## Properties
| Name | Description |
| :- | :- |
|entries|Gets entries of [CpioEntry](/zip/python-net/aspose.zip.cpio/cpioentry/) type constituting the archive.|
|file_entries|Gets entries of [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) type constituting the archive.|
|format|Gets the archive format.|
## Methods
| Name | Description |
| :- | :- |
|create_entry(name, source_path, open_immediately)|Create a single entry within the archive.|
|create_entry(name, source)|Create a single entry within the archive.|
|delete_entry(entry)|Removes the first occurrence of a specific entry from the entry list.|
|delete_entry(entry_index)|Removes the entry from the entry list by index.|
|save(destination_file_name, cpio_format)|Saves archive to a destination file provided.|
|save(output, cpio_format)|Saves archive to the stream provided.|
|save_gzipped(output, cpio_format)|Saves archive to the stream with gzip compression.|
|save_gzipped(path, cpio_format)|Saves archive to the file by path with gzip compression.|
|save_lzipped(output, cpio_format)|Saves archive to the stream with lzip compression.|
|save_lzipped(path, cpio_format)|Saves archive to the file by path with lzip compression.|
|save_lzma_compressed(output, cpio_format)|Saves the archive to the stream with LZMA compression.|
|save_lzma_compressed(path, cpio_format)|Saves the archive to the file by path with lzma compression.|
|save_xz_compressed(output, cpio_format, settings)|Saves archive to the stream with xz compression.|
|save_xz_compressed(path, cpio_format, settings)|Saves archive to the path by path with xz compression.|
|save_z_compressed(output, cpio_format)|Saves archive to the stream with Z compression.|
|save_z_compressed(path, cpio_format)|Saves archive to the path by path with Z compression.|
|save_zstandard(output, cpio_format)|Saves archive to the stream with Zstandard compression.|
|save_zstandard(path, cpio_format)|Saves archive to the file by path with Zstandard compression.|
|create_entries(source_directory, include_root_directory)|Adds to the archive all the files and directories recursively in the directory given.|
|extract_to_directory(destination_directory)|Extracts all the files in the archive to the directory provided.|

### See Also

* namespace [aspose.zip.cpio](/zip/python-net/aspose.zip.cpio/)
* assembly [Aspose.Zip](/zip/python-net/)

