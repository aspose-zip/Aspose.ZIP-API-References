---
title: SplitArchiveSaveOptions.SplitArchiveSaveOptions
second_title: Aspose.ZIP for .NET API 参考
description: SplitArchiveSaveOptions 构造函数. 实例化用于保存多卷 zip 存档的设置
type: docs
weight: 10
url: /zh/net/aspose.zip.saving/splitarchivesaveoptions/splitarchivesaveoptions/
---
## SplitArchiveSaveOptions constructor

实例化用于保存多卷 zip 存档的设置。

```csharp
public SplitArchiveSaveOptions(string fileName, uint segmentSize)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| fileName | String | 卷的名称。可能带有或不带有 .zip 扩展名。 |
| segmentSize | UInt32 | 卷的大小。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentOutOfRangeException | 段大小小于 65536 字节。 |

### 评论

有些体积可能小于*segmentSize*.在大多数情况下，最后一段会更少，但很少有常规段也可能如此。

文件名如下：*fileName* .z01,*fileName* .z02, ...,*fileName* .z(n-1),*fileName*。压缩。

### 也可以看看

* class [SplitArchiveSaveOptions](../)
* 命名空间 [Aspose.Zip.Saving](../../splitarchivesaveoptions/)
* 部件 [Aspose.Zip](../../../)


