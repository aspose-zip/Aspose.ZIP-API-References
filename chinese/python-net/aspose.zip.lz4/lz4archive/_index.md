---
title: "Lz4Archive"
second_title: "Aspose.Zip for Python via .NET API 参考"
description: 
type: docs
weight: 10
url: /zh/python-net/aspose.zip.lz4/lz4archive/
---

## Lz4Archive class

此类表示 LZ4 存档文件。可用于提取或创建 LZ4 存档。

Lz4Archive 类型公开以下成员：
## 构造函数
| 名称 | 描述 |
| :- | :- |
| Lz4Archive(source_stream, load_options) | 初始化一个用于解压的 [Lz4Archive](/zip/python-net/aspose.zip.lz4/lz4archive/) 类的新实例。 |
| Lz4Archive(path, load_options) | 初始化 [Lz4Archive](/zip/python-net/aspose.zip.lz4/lz4archive/) 类的新实例。 |
| Lz4Archive(settings) | 初始化一个用于压缩的 [Lz4Archive](/zip/python-net/aspose.zip.lz4/lz4archive/) 类的新实例。 |
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
| extract(path) | 将存档提取到指定路径的文件中。 |
| extract(destination) | 将存档提取到提供的流中。 |
| save(output) | 将 lz4 存档保存到提供的流中。 |
| save(destination) | 将 lz4 存档保存到提供的目标文件中。 |
| save(destination_file_name) | 将存档保存到提供的目标文件中。 |
| set_source(source) | 设置要在存档中压缩的内容。 |
| set_source(file_info) | 设置要在存档中压缩的内容。 |
| set_source(tar_archive, format) | 设置要在存档中压缩的内容。 |
| set_source(path) | 设置要在存档中压缩的内容。 |
| extract_to_directory(destination_directory) | 将存档的内容提取到提供的目录中。 |
| open() | 打开存档进行提取，并提供包含存档内容的流。 |

### 另请参见

* namespace [aspose.zip.lz4](/zip/python-net/aspose.zip.lz4/)
* assembly [Aspose.Zip](/zip/python-net/)

