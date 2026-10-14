---
title: "Archive"
second_title: "Aspose.Zip for Python via .NET API 参考"
description: 
type: docs
weight: 10
url: /zh/python-net/aspose.zip/archive/
---

## Archive class

此类表示 zip 存档文件。可用于创建、提取或更新 zip 存档。

Archive 类型公开以下成员：
## 构造函数
| 名称 | 描述 |
| :- | :- |
| Archive(new_entry_settings) | 初始化 [Archive](/zip/python-net/aspose.zip/archive/) 类的新实例，并为其条目提供可选设置。 |
| Archive(source_stream, load_options, new_entry_settings) | 初始化 [Archive](/zip/python-net/aspose.zip/archive/) 类的新实例，并构建一个可以从归档中提取的条目列表。 |
| Archive(path, load_options, new_entry_settings) | 初始化 [Archive](/zip/python-net/aspose.zip/archive/) 类的新实例，并构建一个可以从归档中提取的条目列表。 |
| Archive(main_segment, segments_in_order, load_options) | 初始化一个来自多卷 ZIP 存档的 [Archive](/zip/python-net/aspose.zip/archive/) 类的新实例，并构建可从存档中提取的条目列表。 |
## 属性
| 名称 | 描述 |
| :- | :- |
| new_entry_settings | 用于新添加的 [ArchiveEntry](/zip/python-net/aspose.zip/archiveentry/) 项目的压缩和加密设置。 |
| comment | 获取整个存档的注释。 |
| entries | 获取构成存档的 [ArchiveEntry](/zip/python-net/aspose.zip/archiveentry/) 类型的条目。 |
| file_entries | 获取构成存档的 [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) 类型的条目。 |
| format | 获取归档格式。 |
## 方法
| 名称 | 描述 |
| :- | :- |
| create_entry(name, path, open_immediately, new_entry_settings) | 在存档中创建单个条目。 |
| create_entry(name, source, new_entry_settings) | 在存档中创建单个条目。 |
| create_entry(name, file_info, open_immediately, new_entry_settings) | 在存档中创建单个条目。 |
| create_entry(name, source, new_entry_settings, file_info) | 在存档中创建单个条目。 |
| create_entries(directory, include_root_directory) | 将给定目录中的所有文件和子目录递归地添加到存档中。 |
| create_entries(source_directory, include_root_directory) | 将给定目录中的所有文件和子目录递归地添加到存档中。 |
| delete_entry(entry) | 从条目列表中移除特定条目的第一次出现。 |
| delete_entry(entry_index) |  |
| save(output_stream, save_options) | 将存档保存到提供的流中。 |
| save(destination_file_name, save_options) | 将存档保存到提供的目标文件中。 |
| save_split(destination_directory, options) | 将多卷存档保存到提供的目标目录中。 |
| extract_to_directory(destination_directory) | 将存档中的所有文件提取到提供的目录中。 |

### 另请参见

* namespace [aspose.zip](/zip/python-net/aspose.zip/)
* assembly [Aspose.Zip](/zip/python-net/)

