---
title: "LzmaArchive"
second_title: "Aspose.Zip for Python via .NET API 参考"
description: 
type: docs
weight: 10
url: /zh/python-net/aspose.zip.lzma/lzmaarchive/
---

## LzmaArchive class

此类表示 LZMA 存档文件。可用于创建或提取 LZMA 存档。

LzmaArchive 类型公开以下成员：
## 构造函数
| 名称 | 描述 |
| :- | :- |
| LzmaArchive(settings) | 初始化一个 [LzmaArchive](/zip/python-net/aspose.zip.lzma/lzmaarchive/) 类的新实例，并以 lzma 格式创建归档。 |
| LzmaArchive(source) | 初始化一个准备用于解压的 [LzmaArchive](/zip/python-net/aspose.zip.lzma/lzmaarchive/) 类的新实例。 |
| LzmaArchive(path) | 初始化一个准备用于解压的 [LzmaArchive](/zip/python-net/aspose.zip.lzma/lzmaarchive/) 类的新实例。 |
## 属性
| 名称 | 描述 |
| :- | :- |
| file_entries | 获取构成存档的 [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) 类型的条目。 |
| format | 获取归档格式。 |
| name | 获取条目的名称。 |
| length | 获取条目的字节长度。 |
## 方法
| 名称 | 描述 |
| :- | :- |
| extract(destination) | 将 lzma 归档提取到流中。 |
| extract(file_info) | 将 lzma 归档提取到文件中。 |
| extract(path) | 按路径将 lzma 归档提取到文件中。 |
| set_source(source) | 设置要在存档中压缩的内容。 |
| set_source(file_info) | 设置要在存档中压缩的内容。 |
| set_source(source_path) | 设置要在存档中压缩的内容。 |
| save(output) | 将 lzma 归档保存到提供的流中。 |
| save(destination) | 将 lzma 归档保存到提供的目标文件中。 |
| save(destination_file_name) | 将 lzma 归档保存到提供的目标文件中。 |
| extract_to_directory(destination_directory) | 将存档的内容提取到提供的目录中。 |

### 另请参见

* namespace [aspose.zip.lzma](/zip/python-net/aspose.zip.lzma/)
* assembly [Aspose.Zip](/zip/python-net/)

