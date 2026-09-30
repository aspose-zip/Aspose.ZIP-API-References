---
title: "IsoLoadOptions.EntryExtractionProgressed"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Свойство IsoLoadOptions. Получает или задает делегат, вызываемый при извлечении некоторого количества байтов"
type: docs
weight: 30
url: /ru/net/aspose.zip.iso/isoloadoptions/entryextractionprogressed/
---
## IsoLoadOptions.EntryExtractionProgressed property

Получает или задает делегат, вызываемый после извлечения некоторых байтов.

```csharp
public EventHandler<ProgressEventArgs> EntryExtractionProgressed { get; set; }
```

## Примечания

Отправитель события — экземпляр [`IsoEntry`](../../isoentry/), для которого происходит извлечение.

## Примеры

```csharp
IsoArchive archive = new IsoArchive("archive.iso", 
new IsoLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / length); } })                 
```

### См. также

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [IsoLoadOptions](../)
* namespace [Aspose.Zip.Iso](../../isoloadoptions/)
* assembly [Aspose.Zip](../../../)


