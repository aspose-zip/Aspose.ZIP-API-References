---
title: "ParallelOptions.AvailableMemorySize"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Свойство ParallelOptions. Получает или задаёт оценку памяти в мегабайтах, доступную для размещения сжатых записей без выгрузки на диск. Это значение имеет смысл только если настройка ParallelCompressInMemory находится в режиме Auto."
type: docs
weight: 20
url: /ru/net/aspose.zip.saving/paralleloptions/availablememorysize/
---
## ParallelOptions.AvailableMemorySize property

Получает или задаёт оценку памяти в мегабайтах, доступную для размещения сжатых записей без выгрузки на диск. Это значение имеет смысл только если настройка [`ParallelCompressInMemory`](../parallelcompressinmemory/) находится в режиме Auto.

```csharp
public int AvailableMemorySize { get; set; }
```

## Примечания

Это значение используется для расчёта максимального размера записи, которую можно сжимать параллельно с другими. Все записи, превышающие вычисленный порог, будут сжиматься последовательно. Безопасно задавать свойство `AvailableMemorySize` настолько большим, насколько свободно ОЗУ, и даже больше. По умолчанию считается, что у вас есть минимум 200 МБ на каждый ядро процессора.

### См. также

* class [ParallelOptions](../)
* namespace [Aspose.Zip.Saving](../../paralleloptions/)
* assembly [Aspose.Zip](../../../)


