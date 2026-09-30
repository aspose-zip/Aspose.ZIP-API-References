---
title: "AlzEntryEncrypted"
second_title: "Aspose.Zip for Python via .NET API 参考"
description: 
type: docs
weight: 40
url: /zh/python-net/aspose.zip.alz/alzentryencrypted/
---

## AlzEntryEncrypted class

在解压缩前需要解密的 ALZ 条目。

AlzEntryEncrypted 类型公开以下成员：
## 属性
| 名称 | 描述 |
| :- | :- |
| compressed_size | 文件数据的压缩大小（字节）。 |
| uncompressed_size | 文件数据的未压缩大小（字节）。 |
| length | 获取条目的字节长度。 |
| is_directory | 如果此条目表示目录，则返回 true。 |
| name | 文件名（不含路径）。 |
## 方法
| 名称 | 描述 |
| :- | :- |
| extract(path, password) | 将条目提取到提供的路径对应的文件系统中。 |
| extract(destination, password) | 将条目提取到提供的流中。 |
| extract(path) | 将条目提取到提供的路径对应的文件系统中。 |
| extract(destination) | 将条目提取到提供的流中。 |
| open(password) | 打开条目进行提取，并提供一个包含解压后内容的流。 |

### 另请参见

* namespace [aspose.zip.alz](/zip/python-net/aspose.zip.alz/)
* assembly [Aspose.Zip](/zip/python-net/)

