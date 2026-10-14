---
title: "GzipArchive"
second_title: "Aspose.Zip for Python via .NET API 参考"
description: 
type: docs
weight: 10
url: /zh/python-net/aspose.zip.gzip/gziparchive/
---

## GzipArchive class

此类表示 gzip 存档文件。可用于创建或提取 gzip 存档。

GzipArchive 类型公开以下成员：
## 构造函数
| 名称 | 描述 |
| :- | :- |
| GzipArchive() | 初始化一个新的 [GzipArchive](/zip/python-net/aspose.zip.gzip/gziparchive/) 类实例，以进行压缩。 |
| GzipArchive(source_stream, parse_header) | 初始化一个新的 [GzipArchive](/zip/python-net/aspose.zip.gzip/gziparchive/) 类实例，以进行解压缩。 |
| GzipArchive(source_stream, options) | 初始化一个新的 [GzipArchive](/zip/python-net/aspose.zip.gzip/gziparchive/) 类实例，以进行解压缩。 |
| GzipArchive(path, options) | 初始化一个新的 [GzipArchive](/zip/python-net/aspose.zip.gzip/gziparchive/) 类实例，以进行解压缩。 |
| GzipArchive(path, parse_header) | 初始化一个新的 [GzipArchive](/zip/python-net/aspose.zip.gzip/gziparchive/) 类实例，以进行解压缩。 |
## 属性
| 名称 | 描述 |
| :- | :- |
| uncompressed_size | 获取原始文件的大小。 |
| name | 原始文件的名称。 |
| file_entries | 获取构成存档的 [IArchiveFileEntry](/zip/python-net/aspose.zip/iarchivefileentry/) 类型的条目。 |
| format | 获取归档格式。 |
| length | 获取条目的字节长度。 |
## 方法
| 名称 | 描述 |
| :- | :- |
| set_source(source) | 设置要在存档中压缩的内容。 |
| set_source(file_info) | 设置要在存档中压缩的内容。 |
| set_source(path) | 设置要在存档中压缩的内容。 |
| set_source(tar_archive) | 设置要在存档中压缩的内容。 |
| extract(destination) | 将存档提取到提供的流中。 |
| extract(path) | 将存档的内容提取到提供的目录中。 |
| save(output_stream) | 将存档保存到提供的流中。 |
| save(destination_file_name) | 将存档保存到提供的目标文件中。 |
| open() | 打开存档进行提取，并提供包含存档内容的流。 |
| extract_to_directory(destination_directory) | 将存档的内容提取到提供的目录中。 |

### 另请参见

* namespace [aspose.zip.gzip](/zip/python-net/aspose.zip.gzip/)
* assembly [Aspose.Zip](/zip/python-net/)

