---
title: XzBcjX86FilterSettings.XzBcjX86FilterSettings
second_title: Aspose.ZIP untuk Referensi .NET API
description: XzBcjX86FilterSettings konstruktor. Menginisialisasi instance baru dariXzBcjX86FilterSettings . Gunakan untuk mengompres file dan pustaka yang dapat dieksekusi di dalamnyaXzArchive .
type: docs
weight: 10
url: /id/net/aspose.zip.xz.settings/xzbcjx86filtersettings/xzbcjx86filtersettings/
---
## XzBcjX86FilterSettings constructor

Menginisialisasi instance baru dari[`XzBcjX86FilterSettings`](../) . Gunakan untuk mengompres file dan pustaka yang dapat dieksekusi di dalamnya[`XzArchive`](../../../aspose.zip.xz/xzarchive/) .

```csharp
public XzBcjX86FilterSettings()
```

### Contoh

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

### Lihat juga

* class [XzBcjX86FilterSettings](../)
* ruang nama [Aspose.Zip.Xz.Settings](../../xzbcjx86filtersettings/)
* perakitan [Aspose.Zip](../../../)


