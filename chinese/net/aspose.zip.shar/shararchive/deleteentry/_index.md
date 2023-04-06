---
title: SharArchive.DeleteEntry
second_title: Aspose.ZIP for .NET API 参考
description: SharArchive 方法. 从条目列表中删除第一次出现的特定条目
type: docs
weight: 50
url: /zh/net/aspose.zip.shar/shararchive/deleteentry/
---
## DeleteEntry(SharEntry) {#deleteentry}

从条目列表中删除第一次出现的特定条目。

```csharp
public SharArchive DeleteEntry(SharEntry entry)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| entry | SharEntry | 要从条目列表中删除的条目。 |

### 返回值

Shar 条目实例。

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentNullException | *entry*一片空白。 |

### 例子

以下是删除除最后一个条目之外的所有条目的方法：

```csharp
using (var archive = new SharArchive("archive.shar"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save(outputSharFile);
}
```

### 也可以看看

* class [SharEntry](../../sharentry/)
* class [SharArchive](../)
* 命名空间 [Aspose.Zip.Shar](../../shararchive/)
* 部件 [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

按索引从条目列表中删除条目。

```csharp
public SharArchive DeleteEntry(int entryIndex)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| entryIndex | Int32 | 要删除的条目的从零开始的索引。 |

### 返回值

条目已删除的存档。

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentOutOfRangeException | *entryIndex*小于 0.- 或 -*entryIndex*等于或大于`条目`数数。 |

### 例子

```csharp
using (var archive = new SharArchive("two_files.shar"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.shar");
}
```

### 也可以看看

* class [SharArchive](../)
* 命名空间 [Aspose.Zip.Shar](../../shararchive/)
* 部件 [Aspose.Zip](../../../)


