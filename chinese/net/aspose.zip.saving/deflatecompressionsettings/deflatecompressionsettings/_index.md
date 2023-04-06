---
title: DeflateCompressionSettings.DeflateCompressionSettings
second_title: Aspose.ZIP for .NET API 参考
description: DeflateCompressionSettings 构造函数. 初始化一个新的实例DeflateCompressionSettings类.
type: docs
weight: 10
url: /zh/net/aspose.zip.saving/deflatecompressionsettings/deflatecompressionsettings/
---
## DeflateCompressionSettings constructor

初始化一个新的实例[`DeflateCompressionSettings`](../)类.

```csharp
public DeflateCompressionSettings()
```

### 例子

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new DeflateCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### 也可以看看

* class [DeflateCompressionSettings](../)
* 命名空间 [Aspose.Zip.Saving](../../deflatecompressionsettings/)
* 部件 [Aspose.Zip](../../../)


