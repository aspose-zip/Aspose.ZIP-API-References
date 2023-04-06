---
title: PPMdCompressionSettings.PPMdCompressionSettings
second_title: Aspose.ZIP for .NET API 参考
description: PPMdCompressionSettings 构造函数. 初始化一个新的实例PPMdCompressionSettings类.
type: docs
weight: 10
url: /zh/net/aspose.zip.saving/ppmdcompressionsettings/ppmdcompressionsettings/
---
## PPMdCompressionSettings(int, int) {#constructor_1}

初始化一个新的实例[`PPMdCompressionSettings`](../)类.

```csharp
public PPMdCompressionSettings(int modelOrder, int suballocatorSize)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| modelOrder | Int32 | 模型的顺序。 |
| suballocatorSize | Int32 | MB 子分配器中的内存大小可能会消耗。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentOutOfRangeException | *modelOrder*不在 2 到 16 之间。 - 或 -*suballocatorSize*不在 1 到 256 之间。 |

### 评论

更大的模型订单几乎肯定会导致更好的压缩和更多的内存和 CPU 使用率。

PPMd 算法可能需要大量内存，尤其是在用于大文件和/或用于大模型订单时。 如果 ppmd 需要的内存比您提供的多，压缩效果会更差。

### 例子

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings(4, 10))))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### 也可以看看

* class [PPMdCompressionSettings](../)
* 命名空间 [Aspose.Zip.Saving](../../ppmdcompressionsettings/)
* 部件 [Aspose.Zip](../../../)

---

## PPMdCompressionSettings() {#constructor}

初始化一个新的实例[`PPMdCompressionSettings`](../)具有默认模型顺序和子分配器大小的类。

```csharp
public PPMdCompressionSettings()
```

### 评论

默认模型顺序为 8，子分配器大小为 50MB.

### 例子

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### 也可以看看

* class [PPMdCompressionSettings](../)
* 命名空间 [Aspose.Zip.Saving](../../ppmdcompressionsettings/)
* 部件 [Aspose.Zip](../../../)


