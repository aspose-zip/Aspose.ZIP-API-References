---
title: XzCompressionSettings.XzCompressionSettings
second_title: Aspose.ZIP for .NET API 参考
description: XzCompressionSettings 构造函数. 初始化一个新的实例XzCompressionSettings类.
type: docs
weight: 10
url: /zh/net/aspose.zip.saving/xzcompressionsettings/xzcompressionsettings/
---
## XzCompressionSettings constructor

初始化一个新的实例[`XzCompressionSettings`](../)类.

```csharp
public XzCompressionSettings()
```

### 例子

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new XzCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### 也可以看看

* class [XzCompressionSettings](../)
* 命名空间 [Aspose.Zip.Saving](../../xzcompressionsettings/)
* 部件 [Aspose.Zip](../../../)


