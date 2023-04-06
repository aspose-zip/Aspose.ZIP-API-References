---
title: IArchiveFileEntry.Extract
second_title: Aspose.ZIP for .NET API 参考
description: IArchiveFileEntry 方法. 通过提供的路径将条目提取到文件系统
type: docs
weight: 30
url: /zh/net/aspose.zip/iarchivefileentry/extract/
---
## Extract(string) {#extract}

通过提供的路径将条目提取到文件系统。

```csharp
public FileInfo Extract(string path)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| path | String | 目标文件的路径。如果该文件已经存在，它将被覆盖。 |

### 返回值

FileInfo包含提取数据的实例。

### 也可以看看

* interface [IArchiveFileEntry](../)
* 命名空间 [Aspose.Zip](../../iarchivefileentry/)
* 部件 [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

将条目提取到所提供的流中。

```csharp
public void Extract(Stream destination)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| destination | Stream | 目标流。必须是可写的。 |

### 也可以看看

* interface [IArchiveFileEntry](../)
* 命名空间 [Aspose.Zip](../../iarchivefileentry/)
* 部件 [Aspose.Zip](../../../)


