---
title: "Класс ParallelOptions"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Класс Aspose.Zip.Saving.ParallelOptions. Параметры параллельного сжатия"
type: docs
weight: 990
url: /ru/net/aspose.zip.saving/paralleloptions/
---
## ParallelOptions class

Параметры параллельного сжатия.

```csharp
public class ParallelOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [ParallelOptions](paralleloptions/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [AvailableMemorySize](../../aspose.zip.saving/paralleloptions/availablememorysize/) { get; set; } | Получает или задает оценку памяти в мегабайтах, доступную для размещения сжатых записей без выгрузки на диск. Это значение имеет смысл только если параметр [`ParallelCompressInMemory`](./parallelcompressinmemory/) находится в режиме Auto. |
| [ParallelCompressInMemory](../../aspose.zip.saving/paralleloptions/parallelcompressinmemory/) { get; set; } | Получает или задает значение, указывающее, как использовать параллельный подход. |

## Примечания

Эти параметры управляют одновременным сжатием несколькими ядрами процессора.

## Примеры

```csharp
using (var archive = new Archive())
{
    archive.CreateEntries("DirToCompress");
    archive.Save("archive.zip", new ArchiveSaveOptions() { ParallelOptions = new ParallelOptions { ParallelCompressInMemory = ParallelCompressionMode.Auto, AvailableMemorySize = 4000 } });
}
```

### См. также

* namespace [Aspose.Zip.Saving](../../aspose.zip.saving/)
* assembly [Aspose.Zip](../../)


