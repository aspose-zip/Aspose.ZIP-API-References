---
title: XzBcjX86FilterSettings.XzBcjX86FilterSettings
second_title: Aspose.ZIP für .NET-API-Referenz
description: XzBcjX86FilterSettings constructeur. Initialisiert eine neue Instanz vonXzBcjX86FilterSettings . Verwenden Sie es um ausführbare Dateien und Bibliotheken darin zu komprimierenXzArchive .
type: docs
weight: 10
url: /de/net/aspose.zip.xz.settings/xzbcjx86filtersettings/xzbcjx86filtersettings/
---
## XzBcjX86FilterSettings constructor

Initialisiert eine neue Instanz von[`XzBcjX86FilterSettings`](../) . Verwenden Sie es, um ausführbare Dateien und Bibliotheken darin zu komprimieren[`XzArchive`](../../../aspose.zip.xz/xzarchive/) .

```csharp
public XzBcjX86FilterSettings()
```

### Beispiele

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

### Siehe auch

* class [XzBcjX86FilterSettings](../)
* namensraum [Aspose.Zip.Xz.Settings](../../xzbcjx86filtersettings/)
* Montage [Aspose.Zip](../../../)


