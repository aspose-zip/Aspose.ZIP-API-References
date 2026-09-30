---
title: "XarDirectoryEntry"
second_title: "Aspose.Zip for Python via .NET API 参考"
description: 
type: docs
weight: 70
url: /zh/python-net/aspose.zip.xar/xardirectoryentry/
---

## XarDirectoryEntry class

表示 xar 存档中的目录条目。

XarDirectoryEntry 类型公开以下成员：
## 属性
| 名称 | 描述 |
| :- | :- |
| name | 获取存档中条目的名称。 |
| full_path | 获取归档中条目的完整路径。 |
| is_directory | 获取一个值，指示该条目是否表示目录。 |
| parent | 获取条目所属的父目录。 |
| creation_time | 获取文件或目录的创建时间。 |
| last_access_time | 获取文件或目录的最近访问时间。 |
| last_write_time | 获取文件或目录的修改时间。 |
| modification_time | 获取文件或目录的修改时间。 |
| files_and_directories | 获取构成目录的 [XarEntry](/zip/python-net/aspose.zip.xar/xarentry/) 类型的条目。 |
| directories | 获取构成目录的 [XarDirectoryEntry](/zip/python-net/aspose.zip.xar/xardirectoryentry/) 类型的条目。 |
| files | 获取构成目录的 [XarFileEntry](/zip/python-net/aspose.zip.xar/xarfileentry/) 类型的条目。 |
| all_entries | 递归获取构成目录的所有 [XarEntry](/zip/python-net/aspose.zip.xar/xarentry/) 类型的条目。 |
## 方法
| 名称 | 描述 |
| :- | :- |
| extract_to_directory(destination_directory) | 将当前目录中的所有文件提取到提供的目录。 |

### 另请参见

* namespace [aspose.zip.xar](/zip/python-net/aspose.zip.xar/)
* assembly [Aspose.Zip](/zip/python-net/)

