---
title: ArchiveEntry.ExtractionProgressed
second_title: Aspose.ZIP for .NET API 参考
description: ArchiveEntry 事件. 提取原始流的一部分时引发
type: docs
weight: 90
url: /zh/net/aspose.zip/archiveentry/extractionprogressed/
---
## ArchiveEntry.ExtractionProgressed event

提取原始流的一部分时引发。

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

### 评论

事件发送者是[`ArchiveEntry`](../)实例。

### 例子

```csharp
archive.Entries[0].ExtractionProgressed += (s, e) => {  int percent = (int)((100 * e.ProceededBytes) / ((ArchiveEntry)s).UncompressedSize); };
```

### 也可以看看

* class [ProgressEventArgs](../../progresseventargs/)
* class [ArchiveEntry](../)
* 命名空间 [Aspose.Zip](../../archiveentry/)
* 部件 [Aspose.Zip](../../../)


