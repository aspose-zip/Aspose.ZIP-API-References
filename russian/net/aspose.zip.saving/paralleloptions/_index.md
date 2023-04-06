---
title: Class ParallelOptions
second_title: Aspose.ZIP для справочника API .NET
description: Aspose.Zip.Saving.ParallelOptions сорт. Опции для параллельного сжатия.
type: docs
weight: 490
url: /ru/net/aspose.zip.saving/paralleloptions/
---
## ParallelOptions class

Опции для параллельного сжатия.

```csharp
public class ParallelOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [ParallelOptions](paralleloptions/)() | Конструктор по умолчанию. |

## Характеристики

| Имя | Описание |
| --- | --- |
| [AvailableMemorySize](../../aspose.zip.saving/paralleloptions/availablememorysize/) { get; set; } | Получает или задает оценку памяти в мегабайтах, доступную для размещения сжатых записей без свопинга на диск. Это значение имеет смысл, только если[`ParallelCompressInMemory`](./parallelcompressinmemory/) настройка находится вAuto режим. |
| [ParallelCompressInMemory](../../aspose.zip.saving/paralleloptions/parallelcompressinmemory/) { get; set; } | Получает или задает значение, указывающее, как следует использовать параллельный подход. |

### Примечания

Эти параметры управляют одновременным сжатием несколькими ядрами ЦП.

### Примеры

```csharp
using (var archive = new Archive())
{
    archive.CreateEntries("DirToCompress");
    archive.Save("archive.zip", new ArchiveSaveOptions() { ParallelOptions = new ParallelOptions { ParallelCompressInMemory = mode, AvailableMemorySize = 4000 } });
}
```

### Смотрите также

* пространство имен [Aspose.Zip.Saving](../../aspose.zip.saving/)
* сборка [Aspose.Zip](../../)


