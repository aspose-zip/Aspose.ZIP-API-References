---
title: Class SevenZipArchiveEntry
second_title: Aspose.ZIP для справочника API .NET
description: Aspose.Zip.SevenZip.SevenZipArchiveEntry сорт. Представляет один файл в архиве 7z.
type: docs
weight: 670
url: /ru/net/aspose.zip.sevenzip/sevenziparchiveentry/
---
## SevenZipArchiveEntry class

Представляет один файл в архиве 7z.

```csharp
public abstract class SevenZipArchiveEntry : IArchiveFileEntry
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [CompressedSize](../../aspose.zip.sevenzip/sevenziparchiveentry/compressedsize/) { get; } | Получает размер сжатого файла. |
| [CompressionSettings](../../aspose.zip.sevenzip/sevenziparchiveentry/compressionsettings/) { get; } | Получает параметры сжатия или распаковки. |
| [IsDirectory](../../aspose.zip.sevenzip/sevenziparchiveentry/isdirectory/) { get; } | Получает значение, указывающее, представляет ли запись каталог. |
| [ModificationTime](../../aspose.zip.sevenzip/sevenziparchiveentry/modificationtime/) { get; } | Получает дату и время последнего изменения. |
| [Name](../../aspose.zip.sevenzip/sevenziparchiveentry/name/) { get; } | Получает имя записи в архиве. |
| [UncompressedSize](../../aspose.zip.sevenzip/sevenziparchiveentry/uncompressedsize/) { get; } | Получает размер исходного файла. |

## Методы

| Имя | Описание |
| --- | --- |
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/#extract_1)(Stream, string) | Извлекает запись в предоставленный поток. |
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/#extract)(string, string) | Извлекает запись в файловую систему по указанному пути. |
| [Open](../../aspose.zip.sevenzip/sevenziparchiveentry/open/)(string) | Открывает запись для извлечения и предоставляет поток с содержимым записи. |

## События

| Имя | Описание |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip.sevenzip/sevenziparchiveentry/compressionprogressed/) | Возникает при сжатии части необработанного потока. |

### Примечания

Разыграть`SevenZipArchiveEntry` пример для[`SevenZipArchiveEntryEncrypted`](../sevenziparchiveentryencrypted/) чтобы определить, зашифрована ли запись или нет.

### Смотрите также

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* пространство имен [Aspose.Zip.SevenZip](../../aspose.zip.sevenzip/)
* сборка [Aspose.Zip](../../)


