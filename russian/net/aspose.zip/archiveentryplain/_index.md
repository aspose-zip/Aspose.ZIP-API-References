---
title: Class ArchiveEntryPlain
second_title: Aspose.ZIP для справочника API .NET
description: Aspose.Zip.ArchiveEntryPlain сорт. ZIPзапись которую необходимо сжать без шифрования или распаковать без расшифровки.
type: docs
weight: 40
url: /ru/net/aspose.zip/archiveentryplain/
---
## ArchiveEntryPlain class

ZIP-запись, которую необходимо сжать без шифрования или распаковать без расшифровки.

```csharp
public sealed class ArchiveEntryPlain : ArchiveEntry
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
| [Extract](../../aspose.zip/archiveentry/extract/)(Stream, string) | Извлекает запись в предоставленный поток. |
| [Extract](../../aspose.zip/archiveentry/extract/)(string, string) | Извлекает запись в файловую систему по указанному пути. |
| [Open](../../aspose.zip/archiveentry/open/)(string) | Открывает запись для извлечения и предоставляет поток с распакованным содержимым записи. |

## События

| Имя | Описание |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip/archiveentry/compressionprogressed/) | Возникает при сжатии части необработанного потока. |
| event [ExtractionProgressed](../../aspose.zip/archiveentry/extractionprogressed/) | Возникает при извлечении части необработанного потока. |

### Смотрите также

* class [ArchiveEntry](../archiveentry/)
* пространство имен [Aspose.Zip](../../aspose.zip/)
* сборка [Aspose.Zip](../../)


