---
title: CpioArchive.DeleteEntry
second_title: Aspose.ZIP for .NET API 参考
description: CpioArchive 方法. 从条目列表中删除第一次出现的特定条目
type: docs
weight: 50
url: /zh/net/aspose.zip.cpio/cpioarchive/deleteentry/
---
## DeleteEntry(CpioEntry) {#deleteentry}

从条目列表中删除第一次出现的特定条目。

```csharp
public CpioArchive DeleteEntry(CpioEntry entry)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| entry | CpioEntry | 要从条目列表中删除的条目。 |

### 返回值

Cpio 条目实例。

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentNullException | *entry*一片空白。 |

### 例子

以下是删除除最后一个条目之外的所有条目的方法：

```csharp
using (var archive = new CpioArchive("archive.cpio"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save(outputCpioFile);
}
```

### 也可以看看

* class [CpioEntry](../../cpioentry/)
* class [CpioArchive](../)
* 命名空间 [Aspose.Zip.Cpio](../../cpioarchive/)
* 部件 [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

按索引从条目列表中删除条目。

```csharp
public CpioArchive DeleteEntry(int entryIndex)
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
using (var archive = new CpioArchive("two_files.cpio"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.cpio");
}
```

### 也可以看看

* class [CpioArchive](../)
* 命名空间 [Aspose.Zip.Cpio](../../cpioarchive/)
* 部件 [Aspose.Zip](../../../)


