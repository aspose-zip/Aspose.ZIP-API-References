---
title: Class ParallelOptions
second_title: Aspose.ZIP for .NET API 参考
description: Aspose.Zip.Saving.ParallelOptions 班级. 并行压缩选项
type: docs
weight: 490
url: /zh/net/aspose.zip.saving/paralleloptions/
---
## ParallelOptions class

并行压缩选项。

```csharp
public class ParallelOptions
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [ParallelOptions](paralleloptions/)() | 默认构造函数。 |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [AvailableMemorySize](../../aspose.zip.saving/paralleloptions/availablememorysize/) { get; set; } | 获取或设置内存估计（以兆字节为单位）可用于容纳压缩条目而无需交换到磁盘。 此值仅在以下情况下才有意义[`ParallelCompressInMemory`](./parallelcompressinmemory/)设置在Auto模式. |
| [ParallelCompressInMemory](../../aspose.zip.saving/paralleloptions/parallelcompressinmemory/) { get; set; } | 获取或设置指示如何使用并行方法的值。 |

### 评论

这些选项管理多个 CPU 内核的同时压缩。

### 例子

```csharp
using (var archive = new Archive())
{
    archive.CreateEntries("DirToCompress");
    archive.Save("archive.zip", new ArchiveSaveOptions() { ParallelOptions = new ParallelOptions { ParallelCompressInMemory = mode, AvailableMemorySize = 4000 } });
}
```

### 也可以看看

* 命名空间 [Aspose.Zip.Saving](../../aspose.zip.saving/)
* 部件 [Aspose.Zip](../../)


