---
title: XzBcjX86FilterSettings.XzBcjX86FilterSettings
second_title: Aspose.ZIP для справочника API .NET
description: XzBcjX86FilterSettings строитель. Инициализирует новый экземплярXzBcjX86FilterSettings . Используйте его для сжатия исполняемых файлов и библиотек внутриXzArchive .
type: docs
weight: 10
url: /ru/net/aspose.zip.xz.settings/xzbcjx86filtersettings/xzbcjx86filtersettings/
---
## XzBcjX86FilterSettings constructor

Инициализирует новый экземпляр[`XzBcjX86FilterSettings`](../) . Используйте его для сжатия исполняемых файлов и библиотек внутри[`XzArchive`](../../../aspose.zip.xz/xzarchive/) .

```csharp
public XzBcjX86FilterSettings()
```

### Примеры

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

### Смотрите также

* class [XzBcjX86FilterSettings](../)
* пространство имен [Aspose.Zip.Xz.Settings](../../xzbcjx86filtersettings/)
* сборка [Aspose.Zip](../../../)


