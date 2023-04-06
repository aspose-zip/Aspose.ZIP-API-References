---
title: ParallelOptions.AvailableMemorySize
second_title: Aspose.ZIP for .NET API 参考
description: ParallelOptions 财产. 获取或设置内存估计以兆字节为单位可用于容纳压缩条目而无需交换到磁盘 此值仅在以下情况下才有意义ParallelCompressInMemory设置在Auto模式.
type: docs
weight: 20
url: /zh/net/aspose.zip.saving/paralleloptions/availablememorysize/
---
## ParallelOptions.AvailableMemorySize property

获取或设置内存估计（以兆字节为单位）可用于容纳压缩条目而无需交换到磁盘。 此值仅在以下情况下才有意义[`ParallelCompressInMemory`](../parallelcompressinmemory/)设置在Auto模式.

```csharp
public int AvailableMemorySize { get; set; }
```

### 评论

此值用于计算可以与其他条目并行压缩的最大条目大小。超过计算阈值的所有条目将按顺序压缩。 是安全的`AvailableMemorySize`与可用 RAM 一样大甚至更大的财产。默认情况下，假定每个 CPU 内核至少有 200MB。

### 也可以看看

* class [ParallelOptions](../)
* 命名空间 [Aspose.Zip.Saving](../../paralleloptions/)
* 部件 [Aspose.Zip](../../../)


