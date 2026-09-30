---
title: "XarArchive.DeleteEntry"
second_title: "Aspose.ZIP for .NET API 参考"
description: "XarArchive 方法。删除条目列表中首次出现的特定条目"
type: docs
weight: 50
url: /zh/net/aspose.zip.xar/xararchive/deleteentry/
---
## XarArchive.DeleteEntry method

删除条目列表中首次出现的特定条目。

```csharp
public XarArchive DeleteEntry(XarEntry entry)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 条目 | XarEntry | 要从条目列表中删除的条目。 |

### Return Value

Xar 条目实例。

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentNullException | *entry* 为 null。 |
| ObjectDisposedException | 存档已被释放，无法使用。 |
| InvalidOperationException | 存档未打开以进行提取。 |

## 示例

以下是如何删除除最后一个之外的所有条目：

```csharp
using (var archive = new XarArchive("archive.xar"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries.FirstOrDefault());
    archive.Save(outputXarFile);
}
```

### 另请参阅

* class [XarEntry](../../xarentry/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


