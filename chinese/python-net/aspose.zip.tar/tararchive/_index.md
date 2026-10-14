---
title: "TarArchive"
second_title: "Aspose.Zip for Python via .NET API 参考"
description: 
type: docs
weight: 10
url: /zh/python-net/aspose.zip.tar/tararchive/
---

## TarArchive class

此类表示 tar 存档文件。可用于创建、提取或更新 tar 存档。

TarArchive 类型公开以下成员：
## 构造函数
| 名称 | 描述 |
| :- | :- |
| TarArchive() | 初始化一个 [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) 类的新实例。 |
| TarArchive(source_stream) | 初始化 [Archive](/zip/python-net/aspose.zip/archive/) 类的新实例，并构建一个可以从归档中提取的条目列表。 |
| TarArchive(path) | 初始化一个 [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/) 类的实例，并组成一个可从存档中提取的条目列表。 |
## 属性
| 名称 | 描述 |
| :- | :- |
| entries | 获取构成存档的 [TarEntry](/zip/python-net/aspose.zip.tar/tarentry/) 类型的条目。 |
| file_entries | 获取构成存档的 [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) 类型的条目。 |
| format | 获取归档格式。 |
## 方法
| 名称 | 描述 |
| :- | :- |
| create_entry(name, source, file_info) | 在存档中创建单个条目。 |
| create_entry(name, file_info, open_immediately) | 在存档中创建单个条目。 |
| create_entry(name, path, open_immediately) | 在存档中创建单个条目。 |
| create_entries(directory, include_root_directory) | 将给定目录中的所有文件和目录递归地添加到存档中。 |
| create_entries(source_directory, include_root_directory) | 将给定目录中的所有文件和目录递归地添加到存档中。 |
| delete_entry(entry) | 从条目列表中删除特定条目的首次出现。 |
| delete_entry(entry_index) |  |
| save(output, format) |  |
| save(destination_file_name, format) |  |
| save_gzipped(output, format) |  |
| save_gzipped(path, format) |  |
| save_zstandard(output, format) |  |
| save_zstandard(path, format) |  |
| save_lzipped(output, format) |  |
| save_lzipped(path, format) |  |
| save_lzma_compressed(output, format) |  |
| save_lzma_compressed(path, format) |  |
| save_lz4_compressed(output, format) |  |
| save_lz4_compressed(path, format) |  |
| save_xz_compressed(output, format, settings) |  |
| save_xz_compressed(path, format, settings) |  |
| save_z_compressed(output, format) |  |
| save_z_compressed(path, format) |  |
| from_g_zip(source) | 提取提供的 gzip 存档并从提取的数据中组成 [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/)。 |
| from_g_zip(path) | 提取提供的 gzip 存档并从提取的数据中组成 [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/)。 |
| from_zstandard(source) | 提取提供的 Zstandard 存档并从提取的数据中组成 [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/)。 |
| from_zstandard(path) | 提取提供的 Zstandard 存档并从提取的数据中组成 [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/)。 |
| from_l_zip(source) | 提取提供的 lzip 存档并从提取的数据中组成 [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/)。 |
| from_l_zip(path) | 提取提供的 lzip 存档并从提取的数据中组成 [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/)。 |
| from_lzma(source) | 提取提供的 LZMA 存档并从提取的数据中组成 [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/)。 |
| from_lzma(path) | 提取提供的 LZMA 存档并从提取的数据中组成 [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/)。 |
| from_lz4(path) | 提取提供的 LZ4 存档并从提取的数据中组成 [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/)。 |
| from_lz4(source) | 提取提供的 LZ4 存档并从提取的数据中组成 [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/)。 |
| from_xz(source) | 提取提供的 xz 格式存档并从提取的数据中组成 [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/)。 |
| from_xz(path) | 提取提供的 xz 格式存档并从提取的数据中组成 [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/)。 |
| from_z(source) | 提取提供的 Zstandard 存档并从提取的数据中组成 [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/)。 |
| from_z(path) | 提取提供的 Zstandard 存档并从提取的数据中组成 [TarArchive](/zip/python-net/aspose.zip.tar/tararchive/)。 |
| extract_to_directory(destination_directory) | 将存档中的所有文件提取到提供的目录中。 |

### 另请参见

* namespace [aspose.zip.tar](/zip/python-net/aspose.zip.tar/)
* assembly [Aspose.Zip](/zip/python-net/)

