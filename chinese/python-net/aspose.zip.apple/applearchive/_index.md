---
title: "AppleArchive"
second_title: "Aspose.Zip for Python via .NET API 参考"
description: 
type: docs
weight: 10
url: /zh/python-net/aspose.zip.apple/applearchive/
---

## AppleArchive class

此类表示 Apple Archive (.aar) 文件。可用于创建 Apple Archive 文件。

AppleArchive 类型公开以下成员：
## 构造函数
| 名称 | 描述 |
| :- | :- |
| AppleArchive(new_entry_settings) | 使用用于组合条目的设置初始化 [AppleArchive](/zip/python-net/aspose.zip.apple/applearchive/) 类的新实例。 |
| AppleArchive(source_stream, load_options) | 初始化 [AppleArchive](/zip/python-net/aspose.zip.apple/applearchive/) 类的新实例，并组成可从存档中提取的条目列表。 |
| AppleArchive(path, load_options) | 初始化 [AppleArchive](/zip/python-net/aspose.zip.apple/applearchive/) 类的新实例，并组成可从存档中提取的条目列表。 |
## 属性
| 名称 | 描述 |
| :- | :- |
| 条目 | 获取构成存档的条目。 |
| is_solid | 获取一个值，指示归档是否使用固体压缩。<br/>            在固体模式下，所有条目数据被压缩为单一流，并且<br/>            不支持单独提取条目。使用 |
| new_entry_settings | 获取用于新创建条目的设置。 |
| file_entries | 获取构成存档的 [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) 类型的条目。 |
| format | 获取归档格式。 |
## 方法
| 名称 | 描述 |
| :- | :- |
| create_entry(name, path, open_immediately) | 在归档中创建单个条目。 |
| create_entry(name, source) | 在归档中创建单个条目。 |
| create_entry(name, file_info, open_immediately) | 在归档中创建单个条目。 |
| save(output) | 将存档保存到提供的流中。 |
| save(destination_file_name) | 将存档保存到提供的目标文件中。 |
| create_entries(directory, include_root_directory) | 递归地将给定目录中的所有文件和子目录添加到存档中。 |
| extract_to_directory(destination_directory) | 将存档中的所有文件提取到提供的目录中。 |

### 另请参见

* namespace [aspose.zip.apple](/zip/python-net/aspose.zip.apple/)
* assembly [Aspose.Zip](/zip/python-net/)

