---
title: "EggArchive.EggArchive"
second_title: "Aspose.ZIP for .NET API 参考"
description: "EggArchive 构造函数。从流中初始化 EggArchive 类的新实例"
type: docs
weight: 10
url: /zh/net/aspose.zip.egg/eggarchive/eggarchive/
---
## EggArchive(Stream, EggArchiveLoadOptions) {#constructor}

从流中初始化 [`EggArchive`](../) 类的新实例。

```csharp
public EggArchive(Stream stream, EggArchiveLoadOptions loadOptions = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | 流 | EGG 存档流。该流必须支持读取和定位。 |
| loadOptions | EggArchiveLoadOptions | 用于加载存档的选项。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentNullException | *stream* 为 null。 |
| ArgumentException | *stream* 不可读取且不可定位。 |

### 另请参阅

* class [EggArchiveLoadOptions](../../eggarchiveloadoptions/)
* class [EggArchive](../)
* namespace [Aspose.Zip.Egg](../../eggarchive/)
* assembly [Aspose.Zip](../../../)

---

## EggArchive(string, EggArchiveLoadOptions) {#constructor_1}

从文件路径初始化一个新的 [`EggArchive`](../) 类实例。

```csharp
public EggArchive(string path, EggArchiveLoadOptions loadOptions = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 路径 | String | EGG 存档文件的路径。 |
| loadOptions | EggArchiveLoadOptions | 用于加载存档的选项。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentNullException | *path* 为 null。 |
| FileNotFoundException | 文件不存在。 |
| SecurityException | 调用方没有访问所需的权限。 |
| ArgumentException | 该 *path* 为空，仅包含空白字符，或包含无效字符。 |
| UnauthorizedAccessException | 对文件 *path* 的访问被拒绝。 |
| PathTooLongException | 指定的 *path*、文件名或两者均超过系统定义的最大长度。例如，在基于 Windows 的平台上，路径必须少于 248 个字符，文件名必须少于 260 个字符。 |
| NotSupportedException | 位于 *path* 的文件在字符串中间包含冒号 (:)。 |
| FileNotFoundException | 未找到该文件。 |
| DirectoryNotFoundException | 指定的路径无效，例如位于未映射的驱动器上。 |
| IOException | 该文件已打开。 |

### 另请参阅

* class [EggArchiveLoadOptions](../../eggarchiveloadoptions/)
* class [EggArchive](../)
* namespace [Aspose.Zip.Egg](../../eggarchive/)
* assembly [Aspose.Zip](../../../)


