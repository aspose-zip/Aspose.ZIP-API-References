---
title: TarArchive.CreateEntries
second_title: Aspose.ZIP for .NET API 参考
description: TarArchive 方法. 将给定目录中的所有文件和目录递归添加到存档中
type: docs
weight: 70
url: /zh/net/aspose.zip.tar/tararchive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

将给定目录中的所有文件和目录递归添加到存档中。

```csharp
public TarArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| directory | DirectoryInfo | 要压缩的目录。 |
| includeRootDirectory | Boolean | 指示是否包含根目录本身。 |

### 返回值

包含条目的存档。

### 例子

```csharp
using (FileStream tarFile = File.Open("archive.tar", FileMode.Create))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntries(new DirectoryInfo("C:\folder"), false);
        archive.Save(tarFile);
    }
}
```

### 也可以看看

* class [TarArchive](../)
* 命名空间 [Aspose.Zip.Tar](../../tararchive/)
* 部件 [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

将给定目录中的所有文件和目录递归添加到存档中。

```csharp
public TarArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| sourceDirectory | String | 要压缩的目录。 |
| includeRootDirectory | Boolean | 指示是否包含根目录本身。 |

### 返回值

包含条目的存档。

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentNullException | *sourceDirectory*一片空白。 |
| SecurityException | 调用者没有访问所需的权限*sourceDirectory*. |
| ArgumentException | *sourceDirectory*包含无效字符，例如 "、&lt;、&gt; 或 &#x7C;。 |
| PathTooLongException | 指定的路径、文件名或两者都超过了系统定义的最大长度。例如，在基于 Windows 的平台上，路径必须少于 248 个字符，文件名必须少于 260 个字符。指定的路径、文件名或两者都太长。 |

### 例子

```csharp
using (FileStream tarFile = File.Open("archive.tar", FileMode.Create))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntries("C:\folder", false);
        archive.Save(tarFile);
    }
}
```

### 也可以看看

* class [TarArchive](../)
* 命名空间 [Aspose.Zip.Tar](../../tararchive/)
* 部件 [Aspose.Zip](../../../)


