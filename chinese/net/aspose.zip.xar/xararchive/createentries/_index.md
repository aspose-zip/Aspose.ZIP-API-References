---
title: "XarArchive.CreateEntries"
second_title: "Aspose.ZIP for .NET API 参考"
description: "XarArchive 方法。将给定目录中的所有文件和目录递归添加到存档中"
type: docs
weight: 30
url: /zh/net/aspose.zip.xar/xararchive/createentries/
---
## CreateEntries(string, bool, XarCompressionSettings) {#createentries_1}

将给定目录中的所有文件和目录递归添加到存档中。

```csharp
public XarArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true, 
    XarCompressionSettings compressionSettings = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceDirectory | String | 要压缩的目录。 |
| compressionSettings | Boolean | 用于已添加的 [`XarEntry`](../../xarentry/) 项目的压缩设置。 |
| includeRootDirectory | XarCompressionSettings | 指示是否包括根目录本身。 |

### Return Value

Xar 条目实例。

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentNullException | *sourceDirectory* 为 null。 |
| SecurityException | 调用方没有访问 *sourceDirectory* 所需的权限。 |
| ArgumentException | *sourceDirectory* 包含无效字符，例如 \", &lt;, &gt;, 或 &#x7C;。 |
| PathTooLongException | 指定的路径、文件名或两者均超过系统定义的最大长度。例如，在基于 Windows 的平台上，路径必须少于 248 个字符，文件名必须少于 260 个字符。指定的路径、文件名或两者太长。 |
| IOException | *sourceDirectory* 代表一个文件，而不是目录。 |
| ObjectDisposedException | 存档已被释放，无法使用。 |

## 示例

```csharp
using (FileStream xarFile = File.Open("archive.xar", FileMode.Create))
{
    using (var archive = new XarArchive())
    {
        archive.CreateEntries(@"C:\folder", false);
        archive.Save(xarFile);
    }
}
```

### 另请参阅

* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(DirectoryInfo, bool, XarCompressionSettings) {#createentries}

将给定目录中的所有文件和目录递归添加到存档中。

```csharp
public XarArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true, 
    XarCompressionSettings compressionSettings = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| directory | DirectoryInfo | 要压缩的目录。 |
| compressionSettings | Boolean | 用于已添加的 [`XarEntry`](../../xarentry/) 项目的压缩设置。 |
| includeRootDirectory | XarCompressionSettings | 指示是否包括根目录本身。 |

### Return Value

Xar 条目实例。

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentNullException | *directory* 为 null。 |
| SecurityException | 调用者没有访问 *directory* 所需的权限。 |
| IOException | *directory* 代表一个文件，而不是目录。 |
| ObjectDisposedException | 存档已被释放，无法使用。 |

## 示例

```csharp
using (FileStream xarFile = File.Open("archive.xar", FileMode.Create))
{
    using (var archive = new XarArchive())
    {
        archive.CreateEntries(new DirectoryInfo(@"C:\folder"), false);
        archive.Save(xarFile);
    }
}
```

### 另请参阅

* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


