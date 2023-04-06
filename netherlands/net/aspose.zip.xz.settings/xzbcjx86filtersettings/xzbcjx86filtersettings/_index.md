---
title: XzBcjX86FilterSettings.XzBcjX86FilterSettings
second_title: Aspose.ZIP voor .NET API-referentie
description: XzBcjX86FilterSettings constructeur. Initialiseert een nieuw exemplaar van hetXzBcjX86FilterSettings . Gebruik het om uitvoerbare bestanden en bibliotheken erin te comprimerenXzArchive .
type: docs
weight: 10
url: /nl/net/aspose.zip.xz.settings/xzbcjx86filtersettings/xzbcjx86filtersettings/
---
## XzBcjX86FilterSettings constructor

Initialiseert een nieuw exemplaar van het[`XzBcjX86FilterSettings`](../) . Gebruik het om uitvoerbare bestanden en bibliotheken erin te comprimeren[`XzArchive`](../../../aspose.zip.xz/xzarchive/) .

```csharp
public XzBcjX86FilterSettings()
```

### Voorbeelden

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

### Zie ook

* class [XzBcjX86FilterSettings](../)
* naamruimte [Aspose.Zip.Xz.Settings](../../xzbcjx86filtersettings/)
* montage [Aspose.Zip](../../../)


