---
title: WimFileEntry
second_title: Aspose.Zip for Python via .NET API Reference
description: 
type: docs
weight: 40
url: /python-net/aspose.zip.wim/wimfileentry/
---

## WimFileEntry class

Represents single file within wim archive.

The WimFileEntry type exposes the following members:
## Properties
| Name | Description |
| :- | :- |
|archive|Gets the archive the entry belongs to.|
|image|Gets the image the entry belongs to.|
|parent|Gets the parent directory the entry belongs to.|
|name|Gets name of the entry within image.|
|short_name|Gets short name of the entry within image.|
|full_path|Gets full path of the entry within image.|
|change_time|Gets the last time the file or directory was changed.|
|creation_time|Gets the creation time of the file or directory.|
|last_access_time|Gets the last access time of the file or directory.|
|last_write_time|Gets the modification time of the file or directory.|
|alternate_data_streams|Gets the names of the alternate data streams for a file or directory.|
|hard_link|Gets the hardlink id of the file or directory.|
|has_hard_links|Gets whether the file or directory is known by other names.|
|is_directory|Gets a value indicating whether the entry represents directory.|
|length|Gets the length of the entry in bytes.|
## Methods
| Name | Description |
| :- | :- |
|extract(path)|Extracts the entry to the filesystem by the path provided.|
|extract(destination)|Extracts the entry to the stream provided.|
|open()|Opens the entry for extraction and provides a stream with entry content.|

### See Also

* namespace [aspose.zip.wim](/zip/python-net/aspose.zip.wim/)
* assembly [Aspose.Zip](/zip/python-net/)

