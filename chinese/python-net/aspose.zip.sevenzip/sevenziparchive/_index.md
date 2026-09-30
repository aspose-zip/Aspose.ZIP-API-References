---
title: "SevenZipArchive"
second_title: "Aspose.Zip for Python via .NET API 参考"
description: 
type: docs
weight: 10
url: /zh/python-net/aspose.zip.sevenzip/sevenziparchive/
---

## SevenZipArchive class

此类表示 7z 存档文件。可用于创建和提取 7z 存档。

SevenZipArchive 类型公开以下成员：
## 构造函数
| 名称 | 描述 |
| :- | :- |
| SevenZipArchive(new_entry_settings) | 使用可选的条目设置初始化 [SevenZipArchive](/zip/python-net/aspose.zip.sevenzip/sevenziparchive/) 类的新实例。 |
| SevenZipArchive(source_stream, password) | 初始化 [SevenZipArchive](/zip/python-net/aspose.zip.sevenzip/sevenziparchive/) 类的新实例，并构建可从存档中提取的条目列表。 |
| SevenZipArchive(path, password) | 初始化 [SevenZipArchive](/zip/python-net/aspose.zip.sevenzip/sevenziparchive/) 类的新实例，并构建可从存档中提取的条目列表。 |
| SevenZipArchive(source_stream, options) | 初始化 [SevenZipArchive](/zip/python-net/aspose.zip.sevenzip/sevenziparchive/) 类的新实例，并构建可从存档中提取的条目列表。 |
| SevenZipArchive(path, options) | 初始化 [SevenZipArchive](/zip/python-net/aspose.zip.sevenzip/sevenziparchive/) 类的新实例，并构建可从存档中提取的条目列表。 |
| SevenZipArchive(parts, password) | 从多卷 7z 存档初始化 [SevenZipArchive](/zip/python-net/aspose.zip.sevenzip/sevenziparchive/) 类的新实例，并构建可从存档中提取的条目列表。 |
## 属性
| 名称 | 描述 |
| :- | :- |
| new_entry_settings | 用于新添加的 [SevenZipArchiveEntry](/zip/python-net/aspose.zip.sevenzip/sevenziparchiveentry/) 项目的压缩和加密设置。 |
| entries | 获取构成存档的 [SevenZipArchiveEntry](/zip/python-net/aspose.zip.sevenzip/sevenziparchiveentry/) 类型的条目。 |
| file_entries | 获取构成存档的 [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) 类型的条目。 |
| format | 获取归档格式。 |
## 方法
| 名称 | 描述 |
| :- | :- |
| create_entry(name, file_info, open_immediately, new_entry_settings) | 在存档中创建单个条目。 |
| create_entry(name, source, new_entry_settings, file_info) | 在存档中创建单个条目。 |
| create_entry(name, source, new_entry_settings) | 在存档中创建单个条目。 |
| create_entry(name, path, open_immediately, new_entry_settings) | 在存档中创建单个条目。 |
| create_entries(directory, include_root_directory) | 递归地将给定目录中的所有文件和子目录添加到存档中。 |
| create_entries(source_directory, include_root_directory) | 递归地将给定目录中的所有文件和子目录添加到存档中。 |
| save(output, save_options) | 将 7z 存档保存到提供的流中。 |
| save(destination_file_name, save_options) | 将存档保存到提供的目标文件中。 |
| extract_to_directory(destination_directory, password) | 将存档中的所有文件提取到提供的目录中。 |
| extract_to_directory(destination_directory) | 将存档中的所有文件提取到提供的目录中。 |
| save_split(destination_directory, options) | 将多卷存档保存到提供的目标目录中。 |

### 另请参见

* namespace [aspose.zip.sevenzip](/zip/python-net/aspose.zip.sevenzip/)
* assembly [Aspose.Zip](/zip/python-net/)

