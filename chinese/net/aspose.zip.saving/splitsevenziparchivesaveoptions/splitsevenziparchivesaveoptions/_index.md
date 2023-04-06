---
title: SplitSevenZipArchiveSaveOptions.SplitSevenZipArchiveSaveOptions
second_title: Aspose.ZIP for .NET API 参考
description: SplitSevenZipArchiveSaveOptions 构造函数. 实例化用于保存多卷 7z 存档的设置
type: docs
weight: 10
url: /zh/net/aspose.zip.saving/splitsevenziparchivesaveoptions/splitsevenziparchivesaveoptions/
---
## SplitSevenZipArchiveSaveOptions constructor

实例化用于保存多卷 7z 存档的设置。

```csharp
public SplitSevenZipArchiveSaveOptions(string fileName, uint segmentSize)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| fileName | String | 卷的名称。可能带有或不带有 .7z 扩展名。 |
| segmentSize | UInt32 | 卷的大小。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentOutOfRangeException | *segmentSize*小于 100。 |

### 评论

有些体积可能小于*segmentSize*.在大多数情况下，最后一段会更少，但很少有常规段也可能如此。

文件名如下：*fileName* .7z.001,*fileName* .7z.002, ...,*fileName*.7z.(n).

### 也可以看看

* class [SplitSevenZipArchiveSaveOptions](../)
* 命名空间 [Aspose.Zip.Saving](../../splitsevenziparchivesaveoptions/)
* 部件 [Aspose.Zip](../../../)


