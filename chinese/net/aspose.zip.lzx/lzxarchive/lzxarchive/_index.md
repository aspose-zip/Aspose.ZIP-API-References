---
title: "LzxArchive.LzxArchive"
second_title: "Aspose.ZIP for .NET API 参考"
description: "LzxArchive 构造函数。初始化 LzxArchive 类的新实例，并组成可从存档中提取的条目列表"
type: docs
weight: 10
url: /zh/net/aspose.zip.lzx/lzxarchive/lzxarchive/
---
## LzxArchive(Stream, LzxLoadOptions) {#constructor}

初始化 [`LzxArchive`](../) 类的新实例，并组成可从存档中提取的条目列表。

```csharp
public LzxArchive(Stream extractionSource, LzxLoadOptions loadOptions = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| extractionSource | 流 | 存档的来源。 |
| loadOptions | LzxLoadOptions | 用于加载现有存档的选项。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentNullException | *extractionSource* 为 null。 |
| ArgumentException | *extractionSource* 不支持定位。 |
| InvalidDataException | 存档签名错误。- 或 - 文件不是 LZX 存档。 |
| NotImplementedException | Lzx 存档包含合并的条目。 |
| EndOfStreamException | 提供的 *extractionSource* 流太短。 |
| ObjectDisposedException | 当流已关闭时抛出。 |
| IOException | 发生 I/O 错误。 |

## 备注

此构造函数不解压任何条目。请参阅 [`Extract`](../../lzxarchiveentry/extract/) 方法以进行解压。

### 另请参阅

* class [LzxLoadOptions](../../lzxloadoptions/)
* class [LzxArchive](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchive/)
* assembly [Aspose.Zip](../../../)

---

## LzxArchive(string, LzxLoadOptions) {#constructor_1}

初始化 [`LzxArchive`](../) 类的新实例，并组成可从存档中提取的条目列表。

```csharp
public LzxArchive(string path, LzxLoadOptions loadOptions = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 路径 | String | 归档文件的完全限定路径或相对路径。 |
| loadOptions | LzxLoadOptions | 用于加载现有存档的选项。 |

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
| NotImplementedException | Lzx 存档包含合并的条目。 |
| EndOfStreamException | 该文件太短。 |
| ObjectDisposedException | 当流已关闭时抛出。 |

## 备注

此构造函数不解压任何条目。请参阅 [`Extract`](../../lzxarchiveentry/extract/) 方法以进行解压。

## 示例

以下示例提取归档，然后将第一个条目解压到 `MemoryStream`。

```csharp
var extracted = new MemoryStream();
using (LzxArchive archive = new LzxArchive("sample.lzx"))
{
    archive.Entries[0].Extract(extracted);
}
```

### 另请参阅

* class [LzxLoadOptions](../../lzxloadoptions/)
* class [LzxArchive](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchive/)
* assembly [Aspose.Zip](../../../)


