---
title: "Bzip2LoadOptions.ExtractionProgressed"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Событие Bzip2LoadOptions. Событие вызывается, когда извлечено некоторое количество байтов."
type: docs
weight: 30
url: /ru/net/aspose.zip.bzip2/bzip2loadoptions/extractionprogressed/
---
## Bzip2LoadOptions.ExtractionProgressed event

Событие вызывается, когда извлечено некоторое количество байтов.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## Примечания

Отправителем события является экземпляр [`Bzip2Archive`](../../bzip2archive/), процесс извлечения которого продвигается. [`ProceededBytes`](../../../aspose.zip/progresseventargs/proceededbytes/) — количество байтов после извлечения.

## Примеры

```csharp
Bzip2LoadOptions loadOptions = new Bzip2LoadOptions(); 
loadOptions.ExtractionProgressed += (s, e) => { percent = (int) ((double)(100 * e.ProceededBytes) / originalFileLength); };
```

### См. также

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [Bzip2LoadOptions](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2loadoptions/)
* assembly [Aspose.Zip](../../../)


