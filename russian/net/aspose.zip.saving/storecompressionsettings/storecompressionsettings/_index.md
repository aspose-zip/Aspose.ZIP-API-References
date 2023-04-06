---
title: StoreCompressionSettings.StoreCompressionSettings
second_title: Aspose.ZIP для справочника API .NET
description: StoreCompressionSettings строитель. Инициализирует новый экземплярStoreCompressionSettings класс.
type: docs
weight: 10
url: /ru/net/aspose.zip.saving/storecompressionsettings/storecompressionsettings/
---
## StoreCompressionSettings constructor

Инициализирует новый экземпляр[`StoreCompressionSettings`](../) класс.

```csharp
public StoreCompressionSettings()
```

### Примеры

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new StoreCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### Смотрите также

* class [StoreCompressionSettings](../)
* пространство имен [Aspose.Zip.Saving](../../storecompressionsettings/)
* сборка [Aspose.Zip](../../../)


