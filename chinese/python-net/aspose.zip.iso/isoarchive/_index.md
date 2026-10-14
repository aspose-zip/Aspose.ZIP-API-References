---
title: "IsoArchive"
second_title: "Aspose.Zip for Python via .NET API 参考"
description: 
type: docs
weight: 30
url: /zh/python-net/aspose.zip.iso/isoarchive/
---

## IsoArchive class

表示 ISO 归档 (ISO 9660)。

IsoArchive 类型公开以下成员：
## 构造函数
| 名称 | 描述 |
| :- | :- |
| IsoArchive() | 初始化 [IsoArchive](/zip/python-net/aspose.zip.iso/isoarchive/) 类的新实例，并创建一个空的 ISO 存档<br/>             用于添加新文件和目录。 |
| IsoArchive(source_stream, load_options) | 初始化 [IsoArchive](/zip/python-net/aspose.zip.iso/isoarchive/) 类的新实例，并生成可从存档中提取的条目列表。 |
| IsoArchive(path, load_options) | 初始化 [IsoArchive](/zip/python-net/aspose.zip.iso/isoarchive/) 类的新实例，并生成可从存档中提取的条目列表。 |
## 属性
| 名称 | 描述 |
| :- | :- |
| entries | 获取构成存档的 [IsoEntry](/zip/python-net/aspose.zip.iso/isoentry/) 类型的条目。 |
| file_entries | 获取构成存档的 [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) 类型的条目。 |
| format | 获取归档格式。 |
## 方法
| 名称 | 描述 |
| :- | :- |
| create_entry(name, file_path) | 向 ISO 镜像添加文件。 |
| create_entry(name, source) | 向 ISO 镜像添加文件。 |
| create_entry(name) | 向 ISO 镜像添加文件。 |
| save(path, save_options) | 将 ISO 镜像保存到指定路径。 |
| save(stream, save_options) | 将 ISO 镜像保存到指定流。 |
| create_directory(name) | 向 ISO 镜像添加目录。 |
| extract_to_directory(destination_directory) | 将所有条目提取到指定目录。 |

### 另请参见

* namespace [aspose.zip.iso](/zip/python-net/aspose.zip.iso/)
* assembly [Aspose.Zip](/zip/python-net/)

