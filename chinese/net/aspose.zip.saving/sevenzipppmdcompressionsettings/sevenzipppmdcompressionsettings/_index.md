---
title: SevenZipPPMdCompressionSettings.SevenZipPPMdCompressionSettings
second_title: Aspose.ZIP for .NET API 参考
description: SevenZipPPMdCompressionSettings 构造函数. 在 7z 存档中实例化 PPMd 压缩方法的设置
type: docs
weight: 10
url: /zh/net/aspose.zip.saving/sevenzipppmdcompressionsettings/sevenzipppmdcompressionsettings/
---
## SevenZipPPMdCompressionSettings(byte, int) {#constructor_1}

在 7z 存档中实例化 PPMd 压缩方法的设置。

```csharp
public SevenZipPPMdCompressionSettings(byte maxOrder, int suballocatorSize)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| maxOrder | Byte | 最大订单。 |
| suballocatorSize | Int32 | MB 子分配器中的内存大小可能会消耗。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentOutOfRangeException | *maxOrder*不在 2 到 32 之间，或者*suballocatorSize*不在 1 到 1024 之间。 |

### 评论

更大的模型订单几乎肯定会导致更好的压缩和更多的内存和 CPU 使用率。

PPMd 算法可能需要大量内存，尤其是在用于大文件和/或用于大模型订单时。 如果 ppmd 需要的内存比您提供的多，压缩效果会更差。

### 例子

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings(4, 32))))
{
    archive.CreateEntry("data.bin", "data.bin");                        
    archive.Save(sevenZipFile);
 }
```

### 也可以看看

* class [SevenZipPPMdCompressionSettings](../)
* 命名空间 [Aspose.Zip.Saving](../../sevenzipppmdcompressionsettings/)
* 部件 [Aspose.Zip](../../../)

---

## SevenZipPPMdCompressionSettings() {#constructor}

使用默认模型顺序和子分配器大小在 7z 存档中实例化 PPMd 压缩方法的设置。

```csharp
public SevenZipPPMdCompressionSettings()
```

### 评论

默认模型顺序为 6，子分配器大小为 16MB.

### 例子

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                        
    archive.Save(sevenZipFile);
 }
```

### 也可以看看

* class [SevenZipPPMdCompressionSettings](../)
* 命名空间 [Aspose.Zip.Saving](../../sevenzipppmdcompressionsettings/)
* 部件 [Aspose.Zip](../../../)


