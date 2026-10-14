---
title: "ArchiveEntry.ExtractionProgressed"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Событие ArchiveEntry. Вызывается, когда извлечена часть необработанного потока"
type: docs
weight: 100
url: /ru/net/aspose.zip/archiveentry/extractionprogressed/
---
## ArchiveEntry.ExtractionProgressed event

Вызывается, когда часть необработанного потока извлечена.

```csharp
public event EventHandler<ProgressCancelEventArgs> ExtractionProgressed;
```

## Примечания

Отправитель события — экземпляр [`ArchiveEntry`](../). Можно отменить извлечение.

## Примеры

В этом примере обработчик события используется для расчёта доли обработанного размера в процентах.

```csharp
a.Entries[0].ExtractionProgressed += (s, e) => {  int percent = (int)((100 * e.ProceededBytes) / ((ArchiveEntry)s).UncompressedSize); };
```

В этом примере обработчик события используется для отмены после извлечения первых сотен мегабайт элемента.

```csharp
a.Entries[0].ExtractionProgressed += (s, e) => { if (e.ProceededBytes > 100000000) e.Cancel = true; };
```

### См. также

* class [ProgressCancelEventArgs](../../progresscanceleventargs/)
* class [ArchiveEntry](../)
* namespace [Aspose.Zip](../../archiveentry/)
* assembly [Aspose.Zip](../../../)


