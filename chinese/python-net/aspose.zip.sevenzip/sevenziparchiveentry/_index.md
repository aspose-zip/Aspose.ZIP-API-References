---
title: "SevenZipArchiveEntry"
second_title: "Aspose.Zip for Python via .NET API 参考"
description: 
type: docs
weight: 20
url: /zh/python-net/aspose.zip.sevenzip/sevenziparchiveentry/
---

## SevenZipArchiveEntry class

表示 7z 存档中的单个文件。

SevenZipArchiveEntry 类型公开以下成员：
## 属性
| 名称 | 描述 |
| :- | :- |
| name | 获取存档中条目的名称。 |
| modification_time | 获取最后修改的日期和时间。 |
| uncompressed_size | 获取原始文件的大小。 |
| compressed_size | 获取压缩文件的大小。 |
| is_directory | 获取一个值，指示该条目是否表示目录。 |
| compression_settings | 获取压缩或解压缩的设置。 |
| length | 获取条目的字节长度。 |
## 方法
| 名称 | 描述 |
| :- | :- |
| extract(path, password) | 将条目提取到提供的路径对应的文件系统中。 |
| extract(destination, password) | 将条目提取到提供的流中。 |
| extract(path) | 将条目提取到提供的路径对应的文件系统中。 |
| extract(destination) | 将条目提取到提供的流中。 |
| open(password) | 打开条目以进行提取，并提供包含条目内容的流。 |

### 另请参见

* namespace [aspose.zip.sevenzip](/zip/python-net/aspose.zip.sevenzip/)
* assembly [Aspose.Zip](/zip/python-net/)

