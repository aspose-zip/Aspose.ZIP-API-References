---
title: "WimDirectoryEntry"
second_title: "Aspose.Zip for Python via .NET API 参考"
description: 
type: docs
weight: 20
url: /zh/python-net/aspose.zip.wim/wimdirectoryentry/
---

## WimDirectoryEntry class

表示 wim 存档中的单个目录。

WimDirectoryEntry 类型公开以下成员：
## 属性
| 名称 | 描述 |
| :- | :- |
| archive | 获取条目所属的存档。 |
| image | 获取条目所属的映像。 |
| parent | 获取条目所属的父目录。 |
| name | 获取条目在映像中的名称。 |
| short_name | 获取条目在映像中的短名称。 |
| full_path | 获取条目在映像中的完整路径。 |
| change_time | 获取文件或目录上次更改的时间。 |
| creation_time | 获取文件或目录的创建时间。 |
| last_access_time | 获取文件或目录的最近访问时间。 |
| last_write_time | 获取文件或目录的修改时间。 |
| modification_time | 获取文件或目录的修改时间。 |
| alternate_data_streams | 获取文件或目录的备用数据流的名称。 |
| 硬链接 | 获取文件或目录的硬链接 ID。 |
| has_hard_links | 获取文件或目录是否有其他名称。 |
| is_directory | 获取一个值，指示该条目是否表示目录。 |
| directories | 获取构成目录的 [WimDirectoryEntry](/zip/python-net/aspose.zip.wim/wimdirectoryentry/) 类型的条目。 |
| files | 获取构成目录的 [WimFileEntry](/zip/python-net/aspose.zip.wim/wimfileentry/) 类型的条目。 |
| files_and_directories | 获取构成目录的 [WimEntry](/zip/python-net/aspose.zip.wim/wimentry/) 类型的条目。 |
| all_entries | 递归获取构成目录的所有 [WimEntry](/zip/python-net/aspose.zip.wim/wimentry/) 类型的条目。 |
## 方法
| 名称 | 描述 |
| :- | :- |
| extract_to_directory(destination_directory) | 将当前目录中的所有文件提取到提供的目录。 |

### 另请参见

* namespace [aspose.zip.wim](/zip/python-net/aspose.zip.wim/)
* assembly [Aspose.Zip](/zip/python-net/)

