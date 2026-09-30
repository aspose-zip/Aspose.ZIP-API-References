---
title: "CabArchive"
second_title: "Aspose.Zip for Python via .NET API 参考"
description: 
type: docs
weight: 10
url: /zh/python-net/aspose.zip.cab/cabarchive/
---

## CabArchive class

此类表示 CAB 存档文件。

CabArchive 类型公开以下成员：
## 构造函数
| 名称 | 描述 |
| :- | :- |
| CabArchive(settings) | 初始化 [CabArchive](/zip/python-net/aspose.zip.cab/cabarchive/) 类的新实例，用于压缩。 |
| CabArchive(source_stream, load_options) | 初始化 [CabArchive](/zip/python-net/aspose.zip.cab/cabarchive/) 类的新实例，并生成可从存档中提取的条目列表。 |
| CabArchive(path, load_options) | 初始化 [CabArchive](/zip/python-net/aspose.zip.cab/cabarchive/) 类的新实例，并生成可从存档中提取的条目列表。 |
## 属性
| 名称 | 描述 |
| :- | :- |
| entries | 获取构成存档的 [CabEntry](/zip/python-net/aspose.zip.cab/cabentry/) 类型的条目。 |
| file_entries | 获取构成存档的 [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) 类型的条目。 |
| format | 获取归档格式。 |
## 方法
| 名称 | 描述 |
| :- | :- |
| create_entry(name, path, new_entry_settings) | 在存档中创建单个条目。 |
| create_entry(name, source, new_entry_settings) | 在存档中创建单个条目。 |
| create_entry(name, file_info, new_entry_settings) | 在存档中创建单个条目。 |
| create_entries(directory, include_root_directory) | 递归地将指定目录中的所有文件添加到存档中。 |
| create_entries(source_directory, include_root_directory) | 递归地将指定目录路径中的所有文件添加到存档中。 |
| save(output_stream, save_options) | 将存档保存到提供的流中。 |
| save(destination_file_name, save_options) | 将存档保存到提供的目标文件中。 |
| extract_to_directory(destination_directory) | 将存档中的所有文件提取到提供的目录中。 |

### 另请参见

* namespace [aspose.zip.cab](/zip/python-net/aspose.zip.cab/)
* assembly [Aspose.Zip](/zip/python-net/)

