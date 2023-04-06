---
title: XzBcjX86FilterSettings.XzBcjX86FilterSettings
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: XzBcjX86FilterSettings नर्मत. क एक नय उदहरण प्ररंभ करत हैXzBcjX86FilterSettings . नष्पदन यग्य फ़इलं और पुस्तकलयं क भतर से संपड़त करने के लए इसक उपयग करेंXzArchive .
type: docs
weight: 10
url: /hi/net/aspose.zip.xz.settings/xzbcjx86filtersettings/xzbcjx86filtersettings/
---
## XzBcjX86FilterSettings constructor

का एक नया उदाहरण प्रारंभ करता है[`XzBcjX86FilterSettings`](../) . निष्पादन योग्य फ़ाइलों और पुस्तकालयों को भीतर से संपीड़ित करने के लिए इसका उपयोग करें[`XzArchive`](../../../aspose.zip.xz/xzarchive/) .

```csharp
public XzBcjX86FilterSettings()
```

### उदाहरण

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

### यह सभी देखें

* class [XzBcjX86FilterSettings](../)
* नाम स्थान [Aspose.Zip.Xz.Settings](../../xzbcjx86filtersettings/)
* सभा [Aspose.Zip](../../../)


