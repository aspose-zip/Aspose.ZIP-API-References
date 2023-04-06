---
title: XzBcjX86FilterSettings.XzBcjX86FilterSettings
second_title: Aspose.ZIP för .NET API-referens
description: XzBcjX86FilterSettings byggare. Initierar en ny instans avXzBcjX86FilterSettings . Använd den för att komprimera körbara filer och bibliotek inomXzArchive .
type: docs
weight: 10
url: /sv/net/aspose.zip.xz.settings/xzbcjx86filtersettings/xzbcjx86filtersettings/
---
## XzBcjX86FilterSettings constructor

Initierar en ny instans av[`XzBcjX86FilterSettings`](../) . Använd den för att komprimera körbara filer och bibliotek inom[`XzArchive`](../../../aspose.zip.xz/xzarchive/) .

```csharp
public XzBcjX86FilterSettings()
```

### Exempel

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

### Se även

* class [XzBcjX86FilterSettings](../)
* namnutrymme [Aspose.Zip.Xz.Settings](../../xzbcjx86filtersettings/)
* hopsättning [Aspose.Zip](../../../)


