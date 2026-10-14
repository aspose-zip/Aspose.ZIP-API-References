---
title: "XarLoadOptions.EntryExtractionProgressed"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Свойство XarLoadOptions. Возвращает или задает делегат, вызываемый при извлечении некоторых байтов"
type: docs
weight: 30
url: /ru/net/aspose.zip.xar/xarloadoptions/entryextractionprogressed/
---
## XarLoadOptions.EntryExtractionProgressed property

Получает или задает делегат, вызываемый после извлечения некоторых байтов.

```csharp
public EventHandler<ProgressEventArgs> EntryExtractionProgressed { get; set; }
```

## Примечания

Отправитель события — это экземпляр [`XarFileEntry`](../../xarfileentry/), для которого прогресс извлечения.

## Примеры

```csharp
XarArchive archive = new XarArchive("archive.xar", 
new XarLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / ((XarFileEntry)s).Length); } })                 
```

### См. также

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [XarLoadOptions](../)
* namespace [Aspose.Zip.Xar](../../xarloadoptions/)
* assembly [Aspose.Zip](../../../)


