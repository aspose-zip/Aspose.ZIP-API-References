---
title: "XzBcjX86FilterSettings.XzBcjX86FilterSettings"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Конструктор XzBcjX86FilterSettings. Инициализирует новый экземпляр XzBcjX86FilterSettings. Используйте его для сжатия исполняемых файлов и библиотек внутри XzArchive"
type: docs
weight: 10
url: /ru/net/aspose.zip.xz.settings/xzbcjx86filtersettings/xzbcjx86filtersettings/
---
## XzBcjX86FilterSettings constructor

Инициализирует новый экземпляр [`XzBcjX86FilterSettings`](../). Используйте его для сжатия исполняемых файлов и библиотек внутри [`XzArchive`](../../../aspose.zip.xz/xzarchive/).

```csharp
public XzBcjX86FilterSettings()
```

## Примеры

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

### См. также

* class [XzBcjX86FilterSettings](../)
* namespace [Aspose.Zip.Xz.Settings](../../xzbcjx86filtersettings/)
* assembly [Aspose.Zip](../../../)


