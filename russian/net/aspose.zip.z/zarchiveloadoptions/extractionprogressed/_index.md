---
title: "ZArchiveLoadOptions.ExtractionProgressed"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Событие ZArchiveLoadOptions. Получает или задает делегат, вызываемый при извлечении некоторого количества байт"
type: docs
weight: 30
url: /ru/net/aspose.zip.z/zarchiveloadoptions/extractionprogressed/
---
## ZArchiveLoadOptions.ExtractionProgressed event

Получает или задает делегат, вызываемый после извлечения некоторых байтов.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## Примечания

Отправитель события — экземпляр [`ZArchive`](../../zarchive/), у которого происходит прогресс извлечения.

## Примеры

```csharp
ZArchive archive = new ZArchive("archive.z", 
new ZArchiveLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / length); } })
```

### См. также

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZArchiveLoadOptions](../)
* namespace [Aspose.Zip.Z](../../zarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


