---
title: Bzip2CompressionSettings
second_title: Aspose.ZIP for .NET API 参考
description: 初始化Bzip2CompressionSettingsaspose.zip.saving/bzip2compressionsettings类的新实例
type: docs
weight: 10
url: /zh/net/aspose.zip.saving/bzip2compressionsettings/bzip2compressionsettings/
---
## Bzip2CompressionSettings(int) {#constructor_1}

初始化[`Bzip2CompressionSettings`](../../bzip2compressionsettings)类的新实例。

```csharp
public Bzip2CompressionSettings(int blockSize)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| blockSize | Int32 | 块大小以数百千字节为单位。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentOutOfRangeException | 块大小不在 1 和 9 之间。 |

### 例子

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings(1))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### 也可以看看

* class [Bzip2CompressionSettings](../../bzip2compressionsettings)
* 命名空间 [Aspose.Zip.Saving](../../bzip2compressionsettings)
* 部件 [Aspose.Zip](../../../)

---

## Bzip2CompressionSettings() {#constructor}

使用默认块大小初始化[`Bzip2CompressionSettings`](../../bzip2compressionsettings)类的新实例，等于 900 KB。

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

* class [Bzip2CompressionSettings](../../bzip2compressionsettings)
* 命名空间 [Aspose.Zip.Saving](../../bzip2compressionsettings)
* 部件 [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->
