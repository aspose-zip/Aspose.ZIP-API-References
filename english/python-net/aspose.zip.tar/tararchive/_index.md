---
title: TarArchive
second_title: Aspose.Sildes for Python via .NET API Reference
description: 
type: docs
weight: 10
url: /python-net/aspose.zip.tar/tararchive/
---

## TarArchive class

This class represents tar archive file. Use it to compose, extract, or update tar archives.

The TarArchive type exposes the following members:
## Constructors
| Name | Description |
| :- | :- |
|TarArchive()|Initializes a new instance of the [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) class.|
|TarArchive(source_stream)|Initializes a new instance of the TarArchive class|
|TarArchive(path)|Initializes a new instance of the TarArchive class|
## Properties
| Name | Description |
| :- | :- |
|entries|Gets entries of|
|file_entries|Gets entries of|
## Methods
| Name | Description |
| :- | :- |
|delete_entry(entry)|Removes the first occurrence of a specific entry from the entries list.|
|delete_entry(entry_index)|Removes the entry from the entries list by index.|
|save(output, format)|  |
|save(destination_file_name, format)|  |
|save_gzipped(output, format)|  |
|save_gzipped(path, format)|  |
|save_lzipped(output, format)|  |
|save_lzipped(path, format)|  |
|save_xz_compressed(output, format, settings)|  |
|save_xz_compressed(path, format, settings)|  |
|save_z_compressed(output, format)|  |
|save_z_compressed(path, format)|  |
|from_g_zip(source)|Extracts supplied gzip archive and composes|
|from_g_zip(path)|Extracts supplied gzip archive and composes|
|from_l_zip(source)|Extracts supplied lzip archive and composes|
|from_l_zip(path)|Extracts supplied lzip archive and composes|
|from_xz(source)|Extracts supplied xz format archive and composes|
|from_xz(path)|Extracts supplied xz format archive and composes|
|from_z(source)|Extracts supplied Z format archive and composes|
|from_z(path)|Extracts supplied Z format archive and composes|
|create_entry(name, path, open_immediately)|Create single entry within the archive.|
|create_entries(source_directory, include_root_directory)|Adds to the archive all the files and directories recursively in the directory given.|
|extract_to_directory(destination_directory)|Extracts all the files in the archive to the directory provided.|

### See Also

* namespace [aspose.zip.tar](/zip/python-net/aspose.zip.tar/)
* assembly [Aspose.Zip](/zip/python-net/)

