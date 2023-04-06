---
title: Archive.SaveSplit
second_title: Aspose.ZIP for .NET API 参考
description: Archive 方法. 将多卷存档保存到提供的目标目录
type: docs
weight: 100
url: /zh/net/aspose.zip/archive/savesplit/
---
## Archive.SaveSplit method

将多卷存档保存到提供的目标目录。

```csharp
public void SaveSplit(string destinationDirectory, SplitArchiveSaveOptions options)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| destinationDirectory | String | 要创建存档段的目录的路径。 |
| options | SplitArchiveSaveOptions | 存档保存选项，包括文件名。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| InvalidOperationException | 该档案是从现有来源打开的。 |
| NotSupportedException | 这个档案是用 XZ 方法压缩和加密的。 |
| ArgumentNullException | *destinationDirectory*一片空白。 |
| SecurityException | 调用者没有访问目录所需的权限。 |
| ArgumentException | *destinationDirectory*包含无效字符，例如 "、&gt;、&lt; 或 &#x7C;。 |
| PathTooLongException | 指定的路径超过了系统定义的最大长度。 |

### 评论

这个方法组成了几个（`n`) 文件 filename.z01, filename.z02, ..., filename.z(n-1), filename.zip。

不能使现有档案多卷。

### 例子

```csharp
using (Archive archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.SaveSplit(@"C:\Folder",  new SplitArchiveSaveOptions("volume", 65536));
}
```

### 也可以看看

* class [SplitArchiveSaveOptions](../../../aspose.zip.saving/splitarchivesaveoptions/)
* class [Archive](../)
* 命名空间 [Aspose.Zip](../../archive/)
* 部件 [Aspose.Zip](../../../)


