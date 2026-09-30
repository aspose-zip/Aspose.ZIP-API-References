---
title: "XarArchive"
second_title: "Aspose.Zip for Python via .NET API 参考"
description: 
type: docs
weight: 40
url: /zh/python-net/aspose.zip.xar/xararchive/
---

## XarArchive class

此类表示 xar 存档文件。

XarArchive 类型公开以下成员：
## 构造函数
| 名称 | 描述 |
| :- | :- |
| XarArchive(default_compression_settings) | 初始化 [XarArchive](/zip/python-net/aspose.zip.xar/xararchive/) 类的新实例。 |
| XarArchive(source_stream, load_options) | 初始化 [XarArchive](/zip/python-net/aspose.zip.xar/xararchive/) 类的新实例，并组成可从存档中提取的条目列表。 |
| XarArchive(path, load_options) | 初始化 [XarArchive](/zip/python-net/aspose.zip.xar/xararchive/) 类的新实例，并组成可从存档中提取的条目列表。 |
## 属性
| 名称 | 描述 |
| :- | :- |
| entries | 获取构成存档的 [XarEntry](/zip/python-net/aspose.zip.xar/xarentry/) 类型的条目。 |
| file_entries | 获取构成存档的 [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) 类型的条目。 |
| format | 获取归档格式。 |
## 方法
| 名称 | 描述 |
| :- | :- |
| create_entries(source_directory, include_root_directory, compression_settings) | 将给定目录中的所有文件和目录递归地添加到存档中。 |
| create_entries(directory, include_root_directory, compression_settings) | 将给定目录中的所有文件和目录递归地添加到存档中。 |
| create_entry(name, file_info, open_immediately, compression_settings) | 在存档中创建单个条目。 |
| create_entry(name, source_path, open_immediately, compression_settings) | 在存档中创建单个条目。 |
| create_entry(name, source, compression_settings) | 在存档中创建单个条目。 |
| save(destination_file_name, save_options) | 将存档保存到提供的目标文件中。 |
| save(output, save_options) | 将存档保存到提供的流中。 |
| extract_to_directory(destination_directory) | 将存档中的所有文件提取到提供的目录中。 |
| delete_entry(entry) | 从条目列表中删除特定条目的首次出现。 |

### 另请参见

* namespace [aspose.zip.xar](/zip/python-net/aspose.zip.xar/)
* assembly [Aspose.Zip](/zip/python-net/)

