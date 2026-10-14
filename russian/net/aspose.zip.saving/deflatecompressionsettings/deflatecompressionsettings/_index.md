---
title: "DeflateCompressionSettings.DeflateCompressionSettings"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Конструктор DeflateCompressionSettings. Инициализирует новый экземпляр класса DeflateCompressionSettings"
type: docs
weight: 10
url: /ru/net/aspose.zip.saving/deflatecompressionsettings/deflatecompressionsettings/
---
## DeflateCompressionSettings constructor

Инициализирует новый экземпляр класса [`DeflateCompressionSettings`](../).

```csharp
public DeflateCompressionSettings()
```

## Примеры

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new DeflateCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### См. также

* class [DeflateCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../deflatecompressionsettings/)
* assembly [Aspose.Zip](../../../)


