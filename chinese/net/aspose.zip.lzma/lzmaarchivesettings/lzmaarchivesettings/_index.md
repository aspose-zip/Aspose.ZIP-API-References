---
title: LzmaArchiveSettings.LzmaArchiveSettings
second_title: Aspose.ZIP for .NET API 参考
description: LzmaArchiveSettings 构造函数. 初始化一个新的实例LzmaArchiveSettings具有默认字典大小的类等于 16 兆字节.
type: docs
weight: 10
url: /zh/net/aspose.zip.lzma/lzmaarchivesettings/lzmaarchivesettings/
---
## LzmaArchiveSettings constructor

初始化一个新的实例[`LzmaArchiveSettings`](../)具有默认字典大小的类，等于 16 兆字节.

```csharp
public LzmaArchiveSettings()
```

### 例子

```csharp
using (LzmaArchive archive = new LzmaArchive(new LzmaArchiveSettings() { DictionarySize = 1048576 } )
{
    archive.SetSource("data.bin);
    archive.Save(lzmaFile);
}
```

### 也可以看看

* class [LzmaArchiveSettings](../)
* 命名空间 [Aspose.Zip.LZMA](../../lzmaarchivesettings/)
* 部件 [Aspose.Zip](../../../)


