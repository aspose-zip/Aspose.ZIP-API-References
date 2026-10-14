---
title: "XzArchive"
second_title: "Aspose.Zip for Python via .NET API 参考"
description: 
type: docs
weight: 10
url: /zh/python-net/aspose.zip.xz/xzarchive/
---

## XzArchive class

此类表示 xz 存档文件。可用于创建和提取 xz 存档。

XzArchive 类型公开以下成员：
## 构造函数
| 名称 | 描述 |
| :- | :- |
| XzArchive(settings) | 初始化 [XzArchive](/zip/python-net/aspose.zip.xz/xzarchive/) 类的新实例，并以 xz 格式创建归档。 |
| XzArchive(source, options) | 初始化 [XzArchive](/zip/python-net/aspose.zip.xz/xzarchive/) 类的新实例，以进行解压缩。 |
| XzArchive(path, options) | 初始化 [XzArchive](/zip/python-net/aspose.zip.xz/xzarchive/) 类的新实例，以进行解压缩。 |
## 属性
| 名称 | 描述 |
| :- | :- |
| uncompressed_size | 文件数据的未压缩大小（字节）。 |
| file_entries | 获取构成存档的 [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) 类型的条目。 |
| format | 获取归档格式。 |
| name | 获取条目的名称。 |
| length | 获取条目的字节长度。 |
## 方法
| 名称 | 描述 |
| :- | :- |
| extract(destination) | 将 xz 归档提取到流中。 |
| extract(file_info) | 将 xz 归档提取到文件中。 |
| extract(path) | 将存档的内容提取到提供的目录中。 |
| set_source(source) | 设置要在存档中压缩的内容。 |
| set_source(file_info) | 设置要在存档中压缩的内容。 |
| set_source(source_path) | 设置要在存档中压缩的内容。 |
| save(output) | 将 xz 存档保存到提供的流中。 |
| save(destination_file_name) | 将 xz 归档保存到提供的目标文件。 |
| extract_to_directory(destination_directory) | 将存档的内容提取到提供的目录中。 |

### 另请参见

* namespace [aspose.zip.xz](/zip/python-net/aspose.zip.xz/)
* assembly [Aspose.Zip](/zip/python-net/)

