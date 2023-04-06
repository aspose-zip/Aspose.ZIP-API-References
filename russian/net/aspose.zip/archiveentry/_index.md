---
title: Class ArchiveEntry
second_title: Aspose.ZIP для справочника API .NET
description: Aspose.Zip.ArchiveEntry сорт. Представляет один файл в архиве.
type: docs
weight: 20
url: /ru/net/aspose.zip/archiveentry/
---
## ArchiveEntry class

Представляет один файл в архиве.

```csharp
public abstract class ArchiveEntry : IArchiveFileEntry
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [Comment](../../aspose.zip/archiveentry/comment/) { get; } | Получает комментарий к записи в архиве. |
| [CompressedSize](../../aspose.zip/archiveentry/compressedsize/) { get; } | Получает размер сжатого файла. |
| [CompressionSettings](../../aspose.zip/archiveentry/compressionsettings/) { get; } | Получает параметры сжатия или распаковки. |
| [IsDirectory](../../aspose.zip/archiveentry/isdirectory/) { get; } | Получает значение, указывающее, представляет ли запись каталог. |
| [ModificationTime](../../aspose.zip/archiveentry/modificationtime/) { get; set; } | Получает или устанавливает дату и время последнего изменения. |
| [Name](../../aspose.zip/archiveentry/name/) { get; } | Получает имя записи в архиве. |
| [UncompressedSize](../../aspose.zip/archiveentry/uncompressedsize/) { get; } | Получает размер исходного файла. |

## Методы

| Имя | Описание |
| --- | --- |
| [Extract](../../aspose.zip/archiveentry/extract/#extract_1)(Stream, string) | Извлекает запись в предоставленный поток. |
| [Extract](../../aspose.zip/archiveentry/extract/#extract)(string, string) | Извлекает запись в файловую систему по указанному пути. |
| [Open](../../aspose.zip/archiveentry/open/)(string) | Открывает запись для извлечения и предоставляет поток с распакованным содержимым записи. |

## События

| Имя | Описание |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip/archiveentry/compressionprogressed/) | Возникает при сжатии части необработанного потока. |
| event [ExtractionProgressed](../../aspose.zip/archiveentry/extractionprogressed/) | Возникает при извлечении части необработанного потока. |

### Примечания

Разыграть`ArchiveEntry` пример для[`ArchiveEntryEncrypted`](../archiveentryencrypted/) чтобы определить, зашифрована ли запись или нет.

### Смотрите также

* interface [IArchiveFileEntry](../iarchivefileentry/)
* пространство имен [Aspose.Zip](../../aspose.zip/)
* сборка [Aspose.Zip](../../)


