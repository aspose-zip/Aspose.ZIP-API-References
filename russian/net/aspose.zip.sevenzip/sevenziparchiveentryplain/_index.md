---
title: "Класс SevenZipArchiveEntryPlain"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Aspose.Zip.SevenZip.SevenZipArchiveEntryPlain class. Запись SevenZip, которую необходимо сжать без шифрования или распаковать без дешифрования"
type: docs
weight: 1220
url: /ru/net/aspose.zip.sevenzip/sevenziparchiveentryplain/
---
## SevenZipArchiveEntryPlain class

Элемент SevenZip, который необходимо сжать без шифрования или распаковать без дешифрования.

```csharp
public class SevenZipArchiveEntryPlain : SevenZipArchiveEntry
```

## Свойства

| Имя | Описание |
| --- | --- |
| [CompressedSize](../../aspose.zip.sevenzip/sevenziparchiveentry/compressedsize/) { get; } | Получает размер сжатого файла. |
| [CompressionSettings](../../aspose.zip.sevenzip/sevenziparchiveentry/compressionsettings/) { get; } | Возвращает настройки сжатия или распаковки. |
| [IsDirectory](../../aspose.zip.sevenzip/sevenziparchiveentry/isdirectory/) { get; } | Возвращает значение, указывающее, является ли запись каталогом. |
| [ModificationTime](../../aspose.zip.sevenzip/sevenziparchiveentry/modificationtime/) { get; } | Получает дату и время последнего изменения. |
| [Name](../../aspose.zip.sevenzip/sevenziparchiveentry/name/) { get; } | Возвращает имя записи в архиве. |
| [UncompressedSize](../../aspose.zip.sevenzip/sevenziparchiveentry/uncompressedsize/) { get; } | Получает размер оригинального файла. |

## Методы

| Имя | Описание |
| --- | --- |
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/)(Stream, string) | Извлекает запись в предоставленный поток. |
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/)(string, string) | Извлекает запись в файловую систему по указанному пути. |
| [Open](../../aspose.zip.sevenzip/sevenziparchiveentry/open/)(string) | Открывает запись для извлечения и предоставляет поток с содержимым записи. |

## События

| Имя | Описание |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip.sevenzip/sevenziparchiveentry/compressionprogressed/) | Вызывается, когда часть необработанного потока сжата. |

### См. также

* class [SevenZipArchiveEntry](../sevenziparchiveentry/)
* namespace [Aspose.Zip.SevenZip](../../aspose.zip.sevenzip/)
* assembly [Aspose.Zip](../../)


