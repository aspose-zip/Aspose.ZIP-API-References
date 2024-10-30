---
title: Bzip2Archive
second_title: Aspose.Zip for Python via .NET API Reference
description: 
type: docs
weight: 10
url: /python-net/aspose.zip.bzip2/bzip2archive/
---

## Bzip2Archive class

This class represents bzip2 archive file. Use it to compose or extract bzip2 archives.

The Bzip2Archive type exposes the following members:
## Constructors
| Name | Description |
| :- | :- |
|Bzip2Archive()|Initializes a new instance of the|
|Bzip2Archive(source_stream, load_options)|Initializes a new instance of the Bzip2Archive class|
|Bzip2Archive(path, load_options)|Initializes a new instance of the Bzip2Archive class|
## Properties
| Name | Description |
| :- | :- |
|file_entries|Gets entries of [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) type constituting the archive.|
|name|Gets name of the entry.|
|length|Gets the length of the entry in bytes.|
## Methods
| Name | Description |
| :- | :- |
|set_source(source)|Sets the content to be compressed within the archive.|
|set_source(path)|Sets the content to be compressed within the archive.|
|set_source(tar_archive, format)|Sets the content to be compressed within the archive.|
|set_source(cpio_archive, format)|Sets the content to be compressed within the archive.|
|extract(destination)|Extracts the archive to the stream provided.|
|extract(path)|Extracts content of the archive to the directory provided.|
|save(output_stream, save_options)|Saves archive to the stream provided.|
|save(destination_file_name, save_options)|Saves archive to destination file provided.|
|open()|Opens the archive for extraction and provides a stream with archive content.|
|extract_to_directory(destination_directory)|Extracts content of the archive to the directory provided.|

### See Also

* namespace [aspose.zip.bzip2](/zip/python-net/aspose.zip.bzip2/)
* assembly [Aspose.Zip](/zip/python-net/)

