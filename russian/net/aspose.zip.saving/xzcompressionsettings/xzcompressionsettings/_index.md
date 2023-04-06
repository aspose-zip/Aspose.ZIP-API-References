---
title: XzCompressionSettings.XzCompressionSettings
second_title: Aspose.ZIP для справочника API .NET
description: XzCompressionSettings строитель. Инициализирует новый экземплярXzCompressionSettings класс.
type: docs
weight: 10
url: /ru/net/aspose.zip.saving/xzcompressionsettings/xzcompressionsettings/
---
## XzCompressionSettings constructor

Инициализирует новый экземпляр[`XzCompressionSettings`](../) класс.

```csharp
public XzCompressionSettings()
```

### Примеры

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new XzCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Смотрите также

* class [XzCompressionSettings](../)
* пространство имен [Aspose.Zip.Saving](../../xzcompressionsettings/)
* сборка [Aspose.Zip](../../../)


