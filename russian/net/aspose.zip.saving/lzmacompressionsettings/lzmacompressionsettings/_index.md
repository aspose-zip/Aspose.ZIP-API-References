---
title: LzmaCompressionSettings.LzmaCompressionSettings
second_title: Aspose.ZIP для справочника API .NET
description: LzmaCompressionSettings строитель. Инициализирует новый экземплярLzmaCompressionSettingsclass с размером словаря по умолчанию равным 16 мегабайтам.
type: docs
weight: 10
url: /ru/net/aspose.zip.saving/lzmacompressionsettings/lzmacompressionsettings/
---
## LzmaCompressionSettings constructor

Инициализирует новый экземпляр[`LzmaCompressionSettings`](../)class с размером словаря по умолчанию, равным 16 мегабайтам.

```csharp
public LzmaCompressionSettings()
```

### Примеры

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new LzmaCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Смотрите также

* class [LzmaCompressionSettings](../)
* пространство имен [Aspose.Zip.Saving](../../lzmacompressionsettings/)
* сборка [Aspose.Zip](../../../)


