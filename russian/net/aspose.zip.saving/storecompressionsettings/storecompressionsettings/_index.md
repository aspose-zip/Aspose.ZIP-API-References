---
title: "StoreCompressionSettings.StoreCompressionSettings"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Конструктор StoreCompressionSettings. Инициализирует новый экземпляр класса StoreCompressionSettings"
type: docs
weight: 10
url: /ru/net/aspose.zip.saving/storecompressionsettings/storecompressionsettings/
---
## StoreCompressionSettings constructor

Инициализирует новый экземпляр класса [`StoreCompressionSettings`](../).

```csharp
public StoreCompressionSettings()
```

## Примеры

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new StoreCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### См. также

* class [StoreCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../storecompressionsettings/)
* assembly [Aspose.Zip](../../../)


