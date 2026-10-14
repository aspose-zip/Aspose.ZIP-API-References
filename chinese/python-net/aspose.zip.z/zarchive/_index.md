---
title: "ZArchive"
second_title: "Aspose.Zip for Python via .NET API 参考"
description: 
type: docs
weight: 10
url: /zh/python-net/aspose.zip.z/zarchive/
---

## ZArchive class

此类表示 Z（压缩）存档文件。使用它来创建或提取 Z 存档。

ZArchive 类型公开以下成员：
## 构造函数
| 名称 | 描述 |
| :- | :- |
| ZArchive() | 初始化用于压缩的 [ZArchive](/zip/python-net/aspose.zip.z/zarchive/) 类的新实例。 |
| ZArchive(source, load_options) | 初始化用于解压的 [ZArchive](/zip/python-net/aspose.zip.z/zarchive/) 类的新实例。 |
| ZArchive(path, load_options) | 初始化用于解压的 [ZArchive](/zip/python-net/aspose.zip.z/zarchive/) 类的新实例。 |
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
| extract(destination) | 将 Z 存档提取到流中。 |
| extract(file_info) | 将 Z 存档提取到文件中。 |
| extract(path) | 按路径将 Z 存档提取到文件中。 |
| save(output, settings) | 将 xz 存档保存到提供的流中。 |
| save(destination_file_name, settings) | 将 Z 存档保存到提供的目标文件中。 |
| set_source(source) | 设置要在存档中压缩的内容。 |
| set_source(file_info) | 设置要在存档中压缩的内容。 |
| set_source(source_path) | 设置要在存档中压缩的内容。 |
| extract_to_directory(destination_directory) | 将存档的内容提取到提供的目录中。 |

### 另请参见

* namespace [aspose.zip.z](/zip/python-net/aspose.zip.z/)
* assembly [Aspose.Zip](/zip/python-net/)

