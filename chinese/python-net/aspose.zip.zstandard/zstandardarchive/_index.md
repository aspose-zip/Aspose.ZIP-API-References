---
title: "ZstandardArchive"
second_title: "Aspose.Zip for Python via .NET API 参考"
description: 
type: docs
weight: 10
url: /zh/python-net/aspose.zip.zstandard/zstandardarchive/
---

## ZstandardArchive class

此类表示 Zstandard 存档文件。可用于创建 Zstandard 存档。

ZstandardArchive 类型公开以下成员：
## 构造函数
| 名称 | 描述 |
| :- | :- |
| ZstandardArchive() | 初始化用于压缩的 [ZstandardArchive](/zip/python-net/aspose.zip.zstandard/zstandardarchive/) 类的新实例。 |
| ZstandardArchive(source_stream, options) | 初始化用于解压的 [ZstandardArchive](/zip/python-net/aspose.zip.zstandard/zstandardarchive/) 类的新实例。 |
| ZstandardArchive(path, options) | 初始化 [ZstandardArchive](/zip/python-net/aspose.zip.zstandard/zstandardarchive/) 类的新实例。 |
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
| extract(destination) | 将存档提取到提供的流中。 |
| extract(path) | 将存档提取到指定路径的文件中。 |
| set_source(source) | 设置要在存档中压缩的内容。 |
| set_source(file_info) | 设置要在存档中压缩的内容。 |
| set_source(path) | 设置要在存档中压缩的内容。 |
| save(output_stream, settings) | 将存档保存到提供的流中。 |
| save(destination_file_name, settings) | 将存档保存到提供的目标文件中。 |
| save(destination, settings) | 将存档保存到提供的目标文件中。 |
| open() | 打开存档进行提取，并提供包含存档内容的流。 |
| extract_to_directory(destination_directory) | 将存档的内容提取到提供的目录中。 |

### 另请参见

* namespace [aspose.zip.zstandard](/zip/python-net/aspose.zip.zstandard/)
* assembly [Aspose.Zip](/zip/python-net/)

