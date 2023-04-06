---
title: LzmaCompressionSettings.LzmaCompressionSettings
second_title: Aspose.ZIP for .NET API 参考
description: LzmaCompressionSettings 构造函数. 初始化一个新的实例LzmaCompressionSettings具有默认字典大小的类等于 16 兆字节.
type: docs
weight: 10
url: /zh/net/aspose.zip.saving/lzmacompressionsettings/lzmacompressionsettings/
---
## LzmaCompressionSettings constructor

初始化一个新的实例[`LzmaCompressionSettings`](../)具有默认字典大小的类，等于 16 兆字节.

```csharp
public LzmaCompressionSettings()
```

### 例子

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new LzmaCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### 也可以看看

* class [LzmaCompressionSettings](../)
* 命名空间 [Aspose.Zip.Saving](../../lzmacompressionsettings/)
* 部件 [Aspose.Zip](../../../)


