---
title: "UueArchive"
second_title: "Aspose.Zip for Python via .NET API 参考"
description: 
type: docs
weight: 10
url: /zh/python-net/aspose.zip.uue/uuearchive/
---

## UueArchive class

此类表示 uuencoded 文件。

UueArchive 类型公开以下成员：
## 构造函数
| 名称 | 描述 |
| :- | :- |
| UueArchive() | 初始化一个准备进行编码的 [UueArchive](/zip/python-net/aspose.zip.uue/uuearchive/) 类的新实例。 |
| UueArchive(source_stream) | 初始化一个新的 [UueArchive](/zip/python-net/aspose.zip.uue/uuearchive/) 类实例，以进行解码。 |
| UueArchive(path) | 初始化一个新的 [UueArchive](/zip/python-net/aspose.zip.uue/uuearchive/) 类实例。 |
## 属性
| 名称 | 描述 |
| :- | :- |
| name | 原始文件的名称。 |
| file_entries | 获取构成存档的 [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) 类型的条目。 |
| format | 获取归档格式。 |
| length | 获取条目的字节长度。 |
## 方法
| 名称 | 描述 |
| :- | :- |
| save(output_stream, save_options) | 将存档保存到提供的流中。 |
| save(destination_file_name, save_options) | 将存档保存到提供的目标文件中。 |
| extract(destination) | 将存档提取到提供的流中。 |
| extract(path) | 将存档提取到指定路径的文件中。 |
| set_source(source) | 设置要在存档中编码的内容。 |
| set_source(file_info) | 设置要在存档中压缩的内容。 |
| set_source(path) | 设置要在存档中编码的内容。 |
| extract_to_directory(destination_directory) | 将存档的内容提取到提供的目录中。 |
| open() | 打开存档以进行解码，并提供包含存档内容的流。 |

### 另请参见

* namespace [aspose.zip.uue](/zip/python-net/aspose.zip.uue/)
* assembly [Aspose.Zip](/zip/python-net/)

