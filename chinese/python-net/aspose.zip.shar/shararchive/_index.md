---
title: "SharArchive"
second_title: "Aspose.Zip for Python via .NET API 参考"
description: 
type: docs
weight: 10
url: /zh/python-net/aspose.zip.shar/shararchive/
---

## SharArchive class

此类表示 shar 存档文件。

SharArchive 类型公开以下成员：
## 构造函数
| 名称 | 描述 |
| :- | :- |
| SharArchive() | 初始化 [SharArchive](/zip/python-net/aspose.zip.shar/shararchive/) 类的新实例。 |
| SharArchive(path) | 初始化 [SharArchive](/zip/python-net/aspose.zip.shar/shararchive/) 类的新实例，以进行解压缩。 |
## 属性
| 名称 | 描述 |
| :- | :- |
| entries | 获取构成归档的 [SharEntry](/zip/python-net/aspose.zip.shar/sharentry/) 类型的条目。 |
## 方法
| 名称 | 描述 |
| :- | :- |
| create_entries(source_directory, include_root_directory) | 将给定目录中的所有文件和目录递归地添加到存档中。 |
| create_entries(directory, include_root_directory) | 将给定目录中的所有文件和目录递归地添加到存档中。 |
| create_entry(name, file_info, open_immediately) | 在存档中创建单个条目。 |
| create_entry(name, source_path, open_immediately) | 在存档中创建单个条目。 |
| create_entry(name, source) | 在存档中创建单个条目。 |
| delete_entry(entry) | 从条目列表中删除特定条目的首次出现。 |
| delete_entry(entry_index) |  |
| save(destination_file_name) | 将存档保存到提供的目标文件中。 |
| save(output) | 将存档保存到提供的流中。 |

### 另请参见

* namespace [aspose.zip.shar](/zip/python-net/aspose.zip.shar/)
* assembly [Aspose.Zip](/zip/python-net/)

