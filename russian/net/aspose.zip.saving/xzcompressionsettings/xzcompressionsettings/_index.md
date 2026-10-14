---
title: "XzCompressionSettings.XzCompressionSettings"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Конструктор XzCompressionSettings. Инициализирует новый экземпляр класса XzCompressionSettings"
type: docs
weight: 10
url: /ru/net/aspose.zip.saving/xzcompressionsettings/xzcompressionsettings/
---
## XzCompressionSettings constructor

Инициализирует новый экземпляр класса [`XzCompressionSettings`](../).

```csharp
public XzCompressionSettings()
```

## Примеры

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new XzCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### См. также

* class [XzCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../xzcompressionsettings/)
* assembly [Aspose.Zip](../../../)


