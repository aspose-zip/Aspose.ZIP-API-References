---
title: "CabArchive.CreateEntries"
second_title: "Aspose.ZIP for .NET API 参考"
description: "CabArchive 方法。递归地将指定目录中的所有文件添加到存档。"
type: docs
weight: 30
url: /zh/net/aspose.zip.cab/cabarchive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

递归地将指定目录中的所有文件添加到存档。

```csharp
public CabArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| directory | DirectoryInfo | 要压缩的目录。 |
| includeRootDirectory | Boolean | 指示是否在条目路径中包含根目录名称。 |

### Return Value

当前的 [`CabArchive`](../) 实例。

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentNullException | *directory* 为 null。 |
| ObjectDisposedException | 存档已被释放，无法使用。 |
| DirectoryNotFoundException | *directory* 找不到。 |
| SecurityException | 调用方没有访问 *directory* 或其内容所需的权限。 |
| UnauthorizedAccessException | 对 *directory* 或其某个文件的访问被拒绝。 |
| IOException | 访问 *directory* 时出现 I/O 错误。 |
| PathTooLongException | 生成的条目路径超过系统定义的最大长度。 |
| InvalidOperationException | 存档已准备好进行提取，无法添加条目。 |

## 示例

```csharp
using (var archive = new CabArchive())
{
    var directory = new DirectoryInfo("logs");
    archive.CreateEntries(directory);
    archive.Save("logs.cab");
}
```

### 另请参阅

* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

将指定目录路径下的所有文件递归添加到存档中。

```csharp
public CabArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceDirectory | String | 要压缩的目录路径。 |
| includeRootDirectory | Boolean | 指示是否在条目路径中包含根目录名称。 |

### Return Value

当前的 [`CabArchive`](../) 实例。

### 异常

| 异常 | 条件 |
| --- | --- |
| ObjectDisposedException | 存档已被释放，无法使用。 |
| ArgumentNullException | *sourceDirectory* 为 null。 |
| DirectoryNotFoundException | 找不到 *sourceDirectory*。 |
| SecurityException | 调用方没有访问 *sourceDirectory* 所需的权限。 |
| UnauthorizedAccessException | 对 *sourceDirectory* 的访问被拒绝。 |
| PathTooLongException | 指定的 *sourceDirectory* 超过系统定义的最大长度。 |
| ArgumentException | *sourceDirectory* 为空，仅包含空白字符，或包含无效字符。 |
| IOException | 访问 *sourceDirectory* 时出现 I/O 错误。 |
| InvalidOperationException | 存档已准备好进行提取，无法添加条目。 |

## 示例

```csharp
using (var archive = new CabArchive(new CabEntrySettings(new CabStoreCompressionSettings())))
{
    archive.CreateEntries("data", includeRootDirectory: false);
    archive.Save("stored_data.cab");
}
```

### 另请参阅

* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


