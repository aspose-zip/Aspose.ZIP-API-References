---
title: ArchiveLoadOptions.EntryListed
second_title: Aspose.ZIP for .NET API 参考
description: ArchiveLoadOptions 财产. 获取或设置在目录中列出条目时调用的委托
type: docs
weight: 50
url: /zh/net/aspose.zip/archiveloadoptions/entrylisted/
---
## ArchiveLoadOptions.EntryListed property

获取或设置在目录中列出条目时调用的委托。

```csharp
public EventHandler<EntryEventArgs> EntryListed { get; set; }
```

### 例子

```csharp
Archive archive = new Archive("archive.zip", new ArchiveLoadOptions() { EntryListed = (s, e) => { Console.WriteLine(e.Entry.Name); } });
```

### 也可以看看

* class [EntryEventArgs](../../entryeventargs/)
* class [ArchiveLoadOptions](../)
* 命名空间 [Aspose.Zip](../../archiveloadoptions/)
* 部件 [Aspose.Zip](../../../)


