---
title: Archive.DeleteEntry
second_title: Aspose.ZIP for .NET API 参考
description: Archive 方法. 从条目列表中删除第一次出现的特定条目
type: docs
weight: 60
url: /zh/net/aspose.zip/archive/deleteentry/
---
## DeleteEntry(ArchiveEntry) {#deleteentry}

从条目列表中删除第一次出现的特定条目。

```csharp
public Archive DeleteEntry(ArchiveEntry entry)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| entry | ArchiveEntry | 要从条目列表中删除的条目。 |

### 返回值

条目已删除的存档。

### 例子

以下是删除除最后一个条目之外的所有条目的方法：

```csharp
using (var archive = new Archive("archive.zip"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save("last_entry.zip");
}
```

### 也可以看看

* class [ArchiveEntry](../../archiveentry/)
* class [Archive](../)
* 命名空间 [Aspose.Zip](../../archive/)
* 部件 [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

按索引从条目列表中删除条目。

```csharp
public Archive DeleteEntry(int entryIndex)
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
using (var archive = new TarArchive("two_files.zip"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.zip");
}
```

### 也可以看看

* class [Archive](../)
* 命名空间 [Aspose.Zip](../../archive/)
* 部件 [Aspose.Zip](../../../)


