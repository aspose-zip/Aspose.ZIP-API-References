---
title: XzBcjX86FilterSettings.XzBcjX86FilterSettings
second_title: Aspose.ZIP for .NET API Reference
description: XzBcjX86FilterSettings constructor. Initializes a new instance of the XzBcjX86FilterSettings. Use it to compress executable files and libraries within XzArchive
type: docs
weight: 10
url: /net/aspose.zip.xz.settings/xzbcjx86filtersettings/xzbcjx86filtersettings/
---
## XzBcjX86FilterSettings constructor

Initializes a new instance of the [`XzBcjX86FilterSettings`](../). Use it to compress executable files and libraries within [`XzArchive`](../../../aspose.zip.xz/xzarchive/).

```csharp
public XzBcjX86FilterSettings()
```

## Examples

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

### See Also

* class [XzBcjX86FilterSettings](../)
* namespace [Aspose.Zip.Xz.Settings](../../xzbcjx86filtersettings/)
* assembly [Aspose.Zip](../../../)


