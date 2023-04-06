---
title: Bzip2CompressionSettings.Bzip2CompressionSettings
second_title: Aspose.ZIP for .NET API 参考
description: Bzip2CompressionSettings 构造函数. 初始化一个新的实例Bzip2CompressionSettings类.
type: docs
weight: 10
url: /zh/net/aspose.zip.saving/bzip2compressionsettings/bzip2compressionsettings/
---
## Bzip2CompressionSettings(int) {#constructor_1}

初始化一个新的实例[`Bzip2CompressionSettings`](../)类.

```csharp
public Bzip2CompressionSettings(int blockSize)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| blockSize | Int32 | 以数百 KB 为单位的块大小。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentOutOfRangeException | 块大小不在 1 到 9 之间。 |

### 例子

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings(1))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### 也可以看看

* class [Bzip2CompressionSettings](../)
* 命名空间 [Aspose.Zip.Saving](../../bzip2compressionsettings/)
* 部件 [Aspose.Zip](../../../)

---

## Bzip2CompressionSettings() {#constructor}

初始化一个新的实例[`Bzip2CompressionSettings`](../)具有默认块大小的类，等于 900 KB.

```csharp
public Bzip2CompressionSettings()
```

### 例子

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### 也可以看看

* class [Bzip2CompressionSettings](../)
* 命名空间 [Aspose.Zip.Saving](../../bzip2compressionsettings/)
* 部件 [Aspose.Zip](../../../)


