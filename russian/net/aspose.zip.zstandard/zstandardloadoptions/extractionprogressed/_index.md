---
title: "ZstandardLoadOptions.ExtractionProgressed"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Событие ZstandardLoadOptions. Получает или задает делегат, вызываемый при извлечении некоторого количества байтов"
type: docs
weight: 30
url: /ru/net/aspose.zip.zstandard/zstandardloadoptions/extractionprogressed/
---
## ZstandardLoadOptions.ExtractionProgressed event

Получает или задает делегат, вызываемый после извлечения некоторых байтов.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## Примечания

Отправителем события является экземпляр [`ZstandardArchive`](../../zstandardarchive/), прогресс извлечения которого происходит.

## Примеры

```csharp
ZstandardArchive archive = new ZstandardArchive("archive.zst", 
new ZStandardLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / length); } })
```

### См. также

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZstandardLoadOptions](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardloadoptions/)
* assembly [Aspose.Zip](../../../)


