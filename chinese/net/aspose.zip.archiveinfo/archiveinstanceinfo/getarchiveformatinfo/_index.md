---
title: ArchiveInstanceInfo.GetArchiveFormatInfo
second_title: Aspose.ZIP for .NET API 参考
description: ArchiveInstanceInfo 方法. 获取存档格式信息
type: docs
weight: 50
url: /zh/net/aspose.zip.archiveinfo/archiveinstanceinfo/getarchiveformatinfo/
---
## GetArchiveFormatInfo(string) {#getarchiveformatinfo_1}

获取存档格式信息。

```csharp
public static ArchiveFormatInfo GetArchiveFormatInfo(string fileName)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| fileName | String | 存档文件的文件名。 |

### 返回值

有关存档格式的信息，如果未检测到格式，则为 null。

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentNullException | *fileName*一片空白。 |
| SecurityException | 调用者没有所需的访问权限。 |
| ArgumentException | 这*fileName*为空、仅包含空格或包含无效字符。 |
| UnauthorizedAccessException | 访问文件*fileName*被拒绝。 |
| PathTooLongException | 指定的*fileName*超过系统定义的最大长度。例如，在基于 Windows 的平台上，路径必须少于 248 个字符，文件名必须少于 260 个字符。 |
| NotSupportedException | 归档于*fileName*在字符串中间包含一个冒号 (:)。 |
| IOException | 打开文件时发生 I/O 错误。 |

### 也可以看看

* class [ArchiveFormatInfo](../../archiveformatinfo/)
* class [ArchiveInstanceInfo](../)
* 命名空间 [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* 部件 [Aspose.Zip](../../../)

---

## GetArchiveFormatInfo(Stream) {#getarchiveformatinfo}

获取存档格式信息。

```csharp
public static ArchiveFormatInfo GetArchiveFormatInfo(Stream stream)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| stream | Stream | 存档文件的流。 |

### 返回值

有关存档格式的信息，如果未检测到格式，则为 null。

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentNullException | *stream*一片空白。 |
| ArgumentException | *stream*不可搜索。 |

### 也可以看看

* class [ArchiveFormatInfo](../../archiveformatinfo/)
* class [ArchiveInstanceInfo](../)
* 命名空间 [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* 部件 [Aspose.Zip](../../../)


