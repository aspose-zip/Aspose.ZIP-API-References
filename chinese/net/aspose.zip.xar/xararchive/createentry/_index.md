---
title: "XarArchive.CreateEntry"
second_title: "Aspose.ZIP for .NET API 参考"
description: "XarArchive 方法。创建归档中的单个条目"
type: docs
weight: 40
url: /zh/net/aspose.zip.xar/xararchive/createentry/
---
## CreateEntry(string, FileInfo, bool, XarCompressionSettings) {#createentry}

在存档中创建单个条目。

```csharp
public XarEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false, 
    XarCompressionSettings compressionSettings = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| name | String | 条目的名称。 |
| fileInfo | FileInfo | 要压缩的文件或文件夹的元数据。 |
| openImmediately | Boolean | 如果立即打开文件则为 True，否则在存档保存时打开文件。 |
| compressionSettings | XarCompressionSettings | 用于添加的 [`XarEntry`](../../xarentry/) 项目的压缩设置。 |

### Return Value

Xar 条目实例。

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentNullException | *name* 为 null。 |
| ArgumentException | *name* 为空。 |
| ArgumentNullException | *fileInfo* 为 null。 |
| ObjectDisposedException | 存档已被释放，无法使用。 |

## 备注

如果文件使用 *openImmediately* 参数立即打开，它将在归档释放之前被阻塞。

## 示例

```csharp
FileInfo fileInfo = new FileInfo("data.bin");
using (var archive = new XarArchive())
{
    archive.CreateEntry("test.bin", fileInfo);
    archive.Save("archive.xar");
}
```

### 另请参阅

* class [XarEntry](../../xarentry/)
* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool, XarCompressionSettings) {#createentry_2}

在存档中创建单个条目。

```csharp
public XarEntry CreateEntry(string name, string sourcePath, bool openImmediately = false, 
    XarCompressionSettings compressionSettings = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| name | String | 条目的名称。 |
| sourcePath | String | 要压缩的文件路径。 |
| openImmediately | Boolean | 如果立即打开文件则为 True，否则在存档保存时打开文件。 |
| compressionSettings | XarCompressionSettings | 用于添加的 [`XarEntry`](../../xarentry/) 项目的压缩设置。 |

### Return Value

Xar 条目实例。

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentNullException | *sourcePath* 为 null。 |
| SecurityException | 调用方没有访问所需的权限。 |
| ArgumentException | *sourcePath* 为空，仅包含空白字符，或包含无效字符。 - 或者 - 文件名作为 *name* 的一部分，超过 100 个符号。 |
| UnauthorizedAccessException | 对文件 *sourcePath* 的访问被拒绝。 |
| PathTooLongException | 指定的 *sourcePath*、文件名或两者均超过系统定义的最大长度。例如，在基于 Windows 的平台上，路径必须少于 248 个字符，文件名必须少于 260 个字符。 - 或者 - *name* 对于 xar 来说太长。 |
| NotSupportedException | *sourcePath* 处的文件在字符串中间包含冒号 (:)。 |
| InvalidOperationException | 无法修改 xar 存档。 |
| ObjectDisposedException | 存档已被释放，无法使用。 |

## 备注

条目名称仅在 *name* 参数中设置。*sourcePath* 参数提供的文件名不会影响条目名称。

如果文件使用 *openImmediately* 参数立即打开，它将在归档释放之前被阻塞。

## 示例

```csharp
using (var archive = new XarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.xar");
}
```

### 另请参阅

* class [XarEntry](../../xarentry/)
* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, XarCompressionSettings) {#createentry_1}

在存档中创建单个条目。

```csharp
public XarEntry CreateEntry(string name, Stream source, 
    XarCompressionSettings compressionSettings = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| name | String | 条目的名称。 |
| source | 流 | 条目的输入流。 |
| compressionSettings | XarCompressionSettings | 用于添加的 [`XarEntry`](../../xarentry/) 项目的压缩设置。 |

### Return Value

Xar 条目实例。

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentNullException | *name* 为 null。 |
| ArgumentNullException | *source* 为 null。 |
| ArgumentException | *name* 为空。 |
| InvalidOperationException | 无法修改 xar 存档。 |
| ObjectDisposedException | 存档已被释放，无法使用。 |

## 示例

```csharp
using (var archive = new XarArchive())
{
    archive.CreateEntry("data.bin", File.OpenRead("data.bin"));
    archive.Save("archive.xar");
}
```

### 另请参阅

* class [XarEntry](../../xarentry/)
* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


