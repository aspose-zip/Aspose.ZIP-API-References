---
title: "RarArchiveEntry.ExtractionProgressed"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "RarArchiveEntry событие. Вызывается, когда извлечена часть необработанного потока"
type: docs
weight: 80
url: /ru/net/aspose.zip.rar/rararchiveentry/extractionprogressed/
---
## RarArchiveEntry.ExtractionProgressed event

Вызывается, когда часть необработанного потока извлечена.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## Примечания

Отправитель события — экземпляр [`RarArchiveEntry`](../).

## Примеры

```csharp
archive.Entries[0].ExtractionProgressed += (s, e) => {  int percent = (int)((100 * e.ProceededBytes) / ((RarArchiveEntry)s).UncompressedSize); };
```

### См. также

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [RarArchiveEntry](../)
* namespace [Aspose.Zip.Rar](../../rararchiveentry/)
* assembly [Aspose.Zip](../../../)


