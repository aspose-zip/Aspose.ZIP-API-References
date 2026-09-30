---
title: "LhaArchive.LhaArchive"
second_title: "Aspose.ZIP for .NET API 参考"
description: "LhaArchive 构造函数。初始化 LhaArchive 类的新实例，并构建可从存档中提取的条目列表。"
type: docs
weight: 10
url: /zh/net/aspose.zip.lha/lhaarchive/lhaarchive/
---
## LhaArchive(Stream, LhaLoadOptions) {#constructor}

初始化 [`LhaArchive`](../) 类的新实例，并构建可从存档中提取的条目列表。

```csharp
public LhaArchive(Stream sourceStream, LhaLoadOptions loadOptions = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceStream | 流 | 存档的来源。 |
| loadOptions | LhaLoadOptions | 用于加载现有存档的选项。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentNullException | *sourceStream* 为 null |
| ArgumentException | *sourceStream* 不可定位。 |
| InvalidDataException | 发现不适当的数据。 |
| EndOfStreamException | 当在读取预期的字节数之前到达流的末尾时抛出此异常。 |
| ObjectDisposedException | 当对象已被释放时抛出。 |

## 备注

此构造函数不解压任何条目。请参阅[`Extract`](../../lhaarchiveentry/extract/) 方法进行解压。

### 另请参阅

* class [LhaLoadOptions](../../lhaloadoptions/)
* class [LhaArchive](../)
* namespace [Aspose.Zip.Lha](../../lhaarchive/)
* assembly [Aspose.Zip](../../../)

---

## LhaArchive(string, LhaLoadOptions) {#constructor_1}

初始化 [`LhaArchive`](../) 类的新实例，并构建可从存档中提取的条目列表。

```csharp
public LhaArchive(string path, LhaLoadOptions loadOptions = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 路径 | String | 归档文件的完全限定路径或相对路径。 |
| loadOptions | LhaLoadOptions | 用于加载现有存档的选项。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentNullException | *path* 为 null。 |
| SecurityException | 调用方没有访问所需的权限。 |
| ArgumentException | 该 *path* 为空，仅包含空白字符，或包含无效字符。 |
| UnauthorizedAccessException | 对文件 *path* 的访问被拒绝。 |
| PathTooLongException | 指定的 *path*、文件名或两者均超过系统定义的最大长度。例如，在基于 Windows 的平台上，路径必须少于 248 个字符，文件名必须少于 260 个字符。 |
| NotSupportedException | 位于 *path* 的文件在字符串中间包含冒号 (:)。 |
| FileNotFoundException | 未找到该文件。 |
| DirectoryNotFoundException | 指定的路径无效，例如位于未映射的驱动器上。 |
| IOException | 该文件已打开。 |
| InvalidDataException | 文件已损坏。 |
| EndOfStreamException | 当在读取预期的字节数之前到达流的末尾时抛出此异常。 |
| ObjectDisposedException | 当对象已被释放时抛出。 |

## 备注

此构造函数不解压任何条目。请参阅[`Extract`](../../lhaarchiveentry/extract/) 方法进行解压。

## 示例

以下示例提取归档，然后将第一个条目解压到 `MemoryStream`。

```csharp
var extracted = new MemoryStream();
using (LhaArchive archive = new LhaArchive("sample.lzh"))
{
    archive.Entries[0].Extract(extracted);
}
```

### 另请参阅

* class [LhaLoadOptions](../../lhaloadoptions/)
* class [LhaArchive](../)
* namespace [Aspose.Zip.Lha](../../lhaarchive/)
* assembly [Aspose.Zip](../../../)


