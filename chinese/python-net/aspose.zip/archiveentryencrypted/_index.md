---
title: "ArchiveEntryEncrypted"
second_title: "Aspose.Zip for Python via .NET API 参考"
description: 
type: docs
weight: 30
url: /zh/python-net/aspose.zip/archiveentryencrypted/
---

## ArchiveEntryEncrypted class

需要使用加密进行压缩或使用解密进行解压的 Zip 条目。

ArchiveEntryEncrypted 类型公开以下成员：
## 属性
| 名称 | 描述 |
| :- | :- |
| compressed_size | 获取压缩文件的大小。 |
| name | 获取存档中条目的名称。 |
| comment | 获取存档中条目的注释。 |
| uncompressed_size | 获取原始文件的大小。 |
| modification_time | 获取或设置最后修改日期和时间。 |
| is_directory | 获取一个值，指示该条目是否表示目录。 |
| data_source | 如果条目是添加到存档而非提取，则为该条目的来源。 |
| compression_settings | 获取压缩或解压缩的设置。 |
| encryption_settings | 获取加密或解密的设置。 |
| length | 获取条目的字节长度。 |
## 方法
| 名称 | 描述 |
| :- | :- |
| extract(path, password) | 将条目提取到提供的路径对应的文件系统中。 |
| extract(destination, password) | 将条目提取到提供的流中。 |
| extract(path) | 将条目提取到提供的路径对应的文件系统中。 |
| extract(destination) | 将条目提取到提供的流中。 |
| open(password) | 打开条目进行提取，并提供一个包含解压后内容的流。 |

### 另请参见

* namespace [aspose.zip](/zip/python-net/aspose.zip/)
* assembly [Aspose.Zip](/zip/python-net/)

