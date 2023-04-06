---
title: DeflateCompressionSettings.DeflateCompressionSettings
second_title: Aspose.ZIP для справочника API .NET
description: DeflateCompressionSettings строитель. Инициализирует новый экземплярDeflateCompressionSettings класс.
type: docs
weight: 10
url: /ru/net/aspose.zip.saving/deflatecompressionsettings/deflatecompressionsettings/
---
## DeflateCompressionSettings constructor

Инициализирует новый экземпляр[`DeflateCompressionSettings`](../) класс.

```csharp
public DeflateCompressionSettings()
```

### Примеры

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new DeflateCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### Смотрите также

* class [DeflateCompressionSettings](../)
* пространство имен [Aspose.Zip.Saving](../../deflatecompressionsettings/)
* сборка [Aspose.Zip](../../../)


