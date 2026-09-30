---
title: "IsoArchive.CreateEntry"
second_title: "Aspose.ZIP for .NET API 参考"
description: "IsoArchive 方法。向 ISO 镜像添加文件"
type: docs
weight: 40
url: /zh/net/aspose.zip.iso/isoarchive/createentry/
---
## CreateEntry(string, string) {#createentry_2}

向 ISO 镜像添加文件。

```csharp
public IsoEntry CreateEntry(string name, string filePath)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| name | String | ISO 中文件的路径。 |
| 文件路径 | String | 文件的路径。 |

### Return Value

已组成 ISO 条目。

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentNullException | 该 *filePath* 为 null。 |
| ArgumentException | 该 *filePath* 为空，仅包含空白字符，或包含无效字符。 |
| UnauthorizedAccessException | 对文件 *filePath* 的访问被拒绝。 |
| PathTooLongException | 指定的 *filePath* 超过系统定义的最大长度。例如，在基于 Windows 的平台上，路径必须少于 248 个字符，文件名必须少于 260 个字符。 |
| NotSupportedException | 位于 *filePath* 的文件在字符串中间包含冒号 (:)。 |
| IOException | 打开文件时发生 I/O 错误。 |
| ObjectDisposedException | 存档已被释放，无法使用。 |
| DirectoryNotFoundException | 指定的路径无效，（例如，它位于未映射的驱动器上）。 |
| FileNotFoundException | 在 *filePath* 中指定的文件未找到。 |
| InvalidOperationException | 存档未处于编辑模式。 |

### 另请参阅

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream) {#createentry_1}

向 ISO 镜像添加文件。

```csharp
public IsoEntry CreateEntry(string name, Stream source)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| name | String | ISO 中文件的路径。 |
| source | 流 | 包含文件数据的流。 |

### Return Value

已组成 ISO 条目。

### 异常

| 异常 | 条件 |
| --- | --- |
| ObjectDisposedException | 存档已被释放，无法使用。 |
| ArgumentNullException | 当 *name* 或 *source* 为 null 时抛出。 |
| InvalidOperationException | 存档未处于编辑模式。 |

### 另请参阅

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string) {#createentry}

向 ISO 镜像添加文件。

```csharp
public IsoEntry CreateEntry(string name)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| name | String | ISO 中目录的路径。 |

### Return Value

已组成 ISO 条目。

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentNullException | `name` 为 null 或为空。 |
| InvalidOperationException | 存档已打开用于提取。 |
| ObjectDisposedException | 存档已被释放，无法使用。 |

### 另请参阅

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


