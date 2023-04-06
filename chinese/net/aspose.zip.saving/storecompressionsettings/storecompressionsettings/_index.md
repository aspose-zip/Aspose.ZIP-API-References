---
title: StoreCompressionSettings.StoreCompressionSettings
second_title: Aspose.ZIP for .NET API 参考
description: StoreCompressionSettings 构造函数. 初始化一个新的实例StoreCompressionSettings类.
type: docs
weight: 10
url: /zh/net/aspose.zip.saving/storecompressionsettings/storecompressionsettings/
---
## StoreCompressionSettings constructor

初始化一个新的实例[`StoreCompressionSettings`](../)类.

```csharp
public StoreCompressionSettings()
```

### 例子

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new StoreCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### 也可以看看

* class [StoreCompressionSettings](../)
* 命名空间 [Aspose.Zip.Saving](../../storecompressionsettings/)
* 部件 [Aspose.Zip](../../../)


