---
title: "CpioArchive"
second_title: "Aspose.Zip for Python via .NET API 参考"
description: 
type: docs
weight: 10
url: /zh/python-net/aspose.zip.cpio/cpioarchive/
---

## CpioArchive class

此类表示 cpio 存档文件。

CpioArchive 类型公开以下成员：
## 构造函数
| 名称 | 描述 |
| :- | :- |
| CpioArchive() | 初始化 [CpioArchive](/zip/python-net/aspose.zip.cpio/cpioarchive/) 类的新实例。 |
| CpioArchive(source_stream) | 初始化 [CpioArchive](/zip/python-net/aspose.zip.cpio/cpioarchive/) 类的新实例，并构建可从存档中提取的条目列表。 |
| CpioArchive(path) | 初始化 [CpioArchive](/zip/python-net/aspose.zip.cpio/cpioarchive/) 类的新实例，并构建可从存档中提取的条目列表。 |
## 属性
| 名称 | 描述 |
| :- | :- |
| entries | 获取构成存档的 [CpioEntry](/zip/python-net/aspose.zip.cpio/cpioentry/) 类型的条目。 |
| file_entries | 获取构成存档的 [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) 类型的条目。 |
| format | 获取归档格式。 |
## 方法
| 名称 | 描述 |
| :- | :- |
| create_entries(source_directory, include_root_directory) | 将给定目录中的所有文件和目录递归地添加到存档中。 |
| create_entries(directory, include_root_directory) | 将给定目录中的所有文件和目录递归地添加到存档中。 |
| create_entry(name, file_info, open_immediately) | 在存档中创建单个条目。 |
| create_entry(name, source_path, open_immediately) | 在存档中创建单个条目。 |
| create_entry(name, source) | 在存档中创建单个条目。 |
| delete_entry(entry) | 从条目列表中删除特定条目的首次出现。 |
| delete_entry(entry_index) |  |
| save(destination_file_name, cpio_format) | 将存档保存到提供的目标文件中。 |
| save(output, cpio_format) | 将存档保存到提供的流中。 |
| save_gzipped(output, cpio_format) | 使用 gzip 压缩将存档保存到流。 |
| save_gzipped(path, cpio_format) | 使用 gzip 压缩将存档保存到指定路径的文件。 |
| save_lzipped(output, cpio_format) | 使用 lzip 压缩将存档保存到流。 |
| save_lzipped(path, cpio_format) | 使用 lzip 压缩将存档保存到指定路径的文件。 |
| save_lzma_compressed(output, cpio_format) | 使用 LZMA 压缩将存档保存到流。 |
| save_lzma_compressed(path, cpio_format) | 使用 lzma 压缩将存档保存到指定路径的文件。 |
| save_xz_compressed(output, cpio_format, settings) | 使用 xz 压缩将存档保存到流。 |
| save_xz_compressed(path, cpio_format, settings) | 使用 xz 压缩将存档保存到指定路径。 |
| save_z_compressed(output, cpio_format) | 使用 Z 压缩将存档保存到流。 |
| save_z_compressed(path, cpio_format) | 将存档保存到路径，使用 Z 压缩。 |
| save_zstandard(output, cpio_format) | 将存档保存到流中，使用 Zstandard 压缩。 |
| save_zstandard(path, cpio_format) | 将存档保存到指定路径的文件中，使用 Zstandard 压缩。 |
| extract_to_directory(destination_directory) | 将存档中的所有文件提取到提供的目录中。 |

### 另请参见

* namespace [aspose.zip.cpio](/zip/python-net/aspose.zip.cpio/)
* assembly [Aspose.Zip](/zip/python-net/)

