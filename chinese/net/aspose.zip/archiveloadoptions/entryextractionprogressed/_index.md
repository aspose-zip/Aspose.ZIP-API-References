---
title: ArchiveLoadOptions.EntryExtractionProgressed
second_title: Aspose.ZIP for .NET API 参考
description: ArchiveLoadOptions 财产. 获取或设置提取某些字节时调用的委托
type: docs
weight: 40
url: /zh/net/aspose.zip/archiveloadoptions/entryextractionprogressed/
---
## ArchiveLoadOptions.EntryExtractionProgressed property

获取或设置提取某些字节时调用的委托。

```csharp
public EventHandler<ProgressEventArgs> EntryExtractionProgressed { get; set; }
```

### 评论

事件发送者是[`ArchiveEntry`](../../archiveentry/)进行提取的实例。

### 例子

```csharp
Archive archive = new Archive("archive.zip", 
new ArchiveLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / ((ArchiveEntry)s).UncompressedSize); } })                 
```

### 也可以看看

* class [ProgressEventArgs](../../progresseventargs/)
* class [ArchiveLoadOptions](../)
* 命名空间 [Aspose.Zip](../../archiveloadoptions/)
* 部件 [Aspose.Zip](../../../)


