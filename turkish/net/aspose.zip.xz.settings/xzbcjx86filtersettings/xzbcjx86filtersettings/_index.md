---
title: XzBcjX86FilterSettings.XzBcjX86FilterSettings
second_title: Aspose.ZIP for .NET API Referansı
description: XzBcjX86FilterSettings inşaatçı. Yeni bir örneğini başlatır.XzBcjX86FilterSettings . İçindeki yürütülebilir dosyaları ve kitaplıkları sıkıştırmak için kullanınXzArchive .
type: docs
weight: 10
url: /tr/net/aspose.zip.xz.settings/xzbcjx86filtersettings/xzbcjx86filtersettings/
---
## XzBcjX86FilterSettings constructor

Yeni bir örneğini başlatır.[`XzBcjX86FilterSettings`](../) . İçindeki yürütülebilir dosyaları ve kitaplıkları sıkıştırmak için kullanın[`XzArchive`](../../../aspose.zip.xz/xzarchive/) .

```csharp
public XzBcjX86FilterSettings()
```

### Örnekler

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

### Ayrıca bakınız

* class [XzBcjX86FilterSettings](../)
* ad alanı [Aspose.Zip.Xz.Settings](../../xzbcjx86filtersettings/)
* toplantı [Aspose.Zip](../../../)


