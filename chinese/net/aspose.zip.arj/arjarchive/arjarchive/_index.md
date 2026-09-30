---
title: "ArjArchive.ArjArchive"
second_title: "Aspose.ZIP for .NET API 参考"
description: "ArjArchive 构造函数。初始化 ArjArchive 类的新实例并构建可从存档中提取的条目列表"
type: docs
weight: 10
url: /zh/net/aspose.zip.arj/arjarchive/arjarchive/
---
## ArjArchive(Stream, ArjLoadOptions) {#constructor}

初始化 [`ArjArchive`](../) 类的新实例并构建可从存档中提取的条目列表。

```csharp
public ArjArchive(Stream extractionSource, ArjLoadOptions loadOptions = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| extractionSource | 流 | 存档的来源。 |
| loadOptions | ArjLoadOptions | 用于加载现有存档的选项。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentNullException | *extractionSource* 为 null。 |
| ArgumentException | &gt;*extractionSource* 不支持定位。 |
| InvalidDataException | 存档签名错误。- 或 - 文件不是 ARJ 存档。 |
| EndOfStreamException | 当在读取所有头字节或名称字节之前到达流的末尾时抛出此异常。 |
| NotSupportedException | 归档已损坏。 |

## 备注

此构造函数不解压任何条目。请参阅[`Extract`](../../arjentryplain/extract/) 方法进行解压。

### 另请参阅

* class [ArjLoadOptions](../../arjloadoptions/)
* class [ArjArchive](../)
* namespace [Aspose.Zip.Arj](../../arjarchive/)
* assembly [Aspose.Zip](../../../)

---

## ArjArchive(string, ArjLoadOptions) {#constructor_1}

初始化 [`ArjArchive`](../) 类的新实例并构建可从存档中提取的条目列表。

```csharp
public ArjArchive(string path, ArjLoadOptions loadOptions = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 路径 | String | 存档文件的路径。 |
| loadOptions | ArjLoadOptions | 用于加载现有存档的选项。 |

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
| EndOfStreamException | 当在读取所有头字节或名称字节之前到达流的末尾时抛出此异常。 |
| InvalidDataException | ARJ 魔数无效或头部大小超出范围。 |

## 备注

此构造函数不解包任何条目。请参阅[`Extract`](../../arjentryplain/extract/) 方法进行解压。

## 示例

下面的示例展示了如何将所有条目提取到目录中。

```csharp
using (var archive = new ArjArchive("archive.arj")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### 另请参阅

* class [ArjLoadOptions](../../arjloadoptions/)
* class [ArjArchive](../)
* namespace [Aspose.Zip.Arj](../../arjarchive/)
* assembly [Aspose.Zip](../../../)


