---
title: XzBcjX86FilterSettings.XzBcjX86FilterSettings
second_title: Aspose.ZIP for .NET API 参考
description: XzBcjX86FilterSettings 构造函数. 初始化一个新的实例XzBcjX86FilterSettings .使用它来压缩其中的可执行文件和库XzArchive .
type: docs
weight: 10
url: /zh/net/aspose.zip.xz.settings/xzbcjx86filtersettings/xzbcjx86filtersettings/
---
## XzBcjX86FilterSettings constructor

初始化一个新的实例[`XzBcjX86FilterSettings`](../) .使用它来压缩其中的可执行文件和库[`XzArchive`](../../../aspose.zip.xz/xzarchive/) .

```csharp
public XzBcjX86FilterSettings()
```

### 例子

```csharp
XzLZMA2FilterSettings lzma2 = new XzLZMA2FilterSettings(5242880);
XzBcjX86FilterSettings bcj = new XzBcjX86FilterSettings();
XzArchiveSettings settings = new XzArchiveSettings(new XzFilterSettings[] {bcj,lzma2}, 10485760, XzCheckType.Crc32);
using (XzArchive archive = new XzArchive(settings))
{
    archive.SetSource("data.bin");
    archive.Save("archive.xz");
}
```

### 也可以看看

* class [XzBcjX86FilterSettings](../)
* 命名空间 [Aspose.Zip.Xz.Settings](../../xzbcjx86filtersettings/)
* 部件 [Aspose.Zip](../../../)


