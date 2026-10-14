---
title: "WimArchive"
second_title: "Aspose.Zip for Python via .NET API 参考"
description: 
type: docs
weight: 10
url: /zh/python-net/aspose.zip.wim/wimarchive/
---

## WimArchive class

此类表示 wim 存档文件。

WimArchive 类型公开以下成员：
## 构造函数
| 名称 | 描述 |
| :- | :- |
| WimArchive(source_stream, load_options) | 初始化 [WimArchive](/zip/python-net/aspose.zip.wim/wimarchive/) 类的新实例，并构建可从存档中提取的条目列表。 |
| WimArchive(path, load_options) | 初始化 [WimArchive](/zip/python-net/aspose.zip.wim/wimarchive/) 类的新实例，并构建可从存档中提取的条目列表。 |
## 属性
| 名称 | 描述 |
| :- | :- |
| images | 获取构成存档的 [WimImage](/zip/python-net/aspose.zip.wim/wimimage/) 类型的条目。 |
| entries | 获取构成存档的 [WimEntry](/zip/python-net/aspose.zip.wim/wimentry/) 类型的条目。 |
| guid | 获取存档的标识 GUID。 |
| boot_image_index | 获取可启动映像的（从零开始的）索引。 |
| file_format_version | 获取文件格式的版本。 |
| manifest | 获取描述文件及其包含的映像的嵌入式清单。 |
| file_entries | 获取构成存档的 [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) 类型的条目。 |
| format | 获取归档格式。 |
## 方法
| 名称 | 描述 |
| :- | :- |
| extract_to_directory(destination_directory) | 将存档提取到指定路径的文件中。 |

### 另请参见

* namespace [aspose.zip.wim](/zip/python-net/aspose.zip.wim/)
* assembly [Aspose.Zip](/zip/python-net/)

