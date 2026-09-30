---
title: "Класс ArchiveEntry"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Класс Aspose.Zip.ArchiveEntry. Представляет отдельный файл в архиве"
type: docs
weight: 170
url: /ru/net/aspose.zip/archiveentry/
---
## ArchiveEntry class

Представляет отдельный файл в архиве.

```csharp
public abstract class ArchiveEntry : IArchiveFileEntry
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Comment](../../aspose.zip/archiveentry/comment/) { get; } | Возвращает комментарий записи в архиве. |
| [CompressedSize](../../aspose.zip/archiveentry/compressedsize/) { get; } | Возвращает размер сжатого файла. |
| [CompressionSettings](../../aspose.zip/archiveentry/compressionsettings/) { get; } | Возвращает настройки сжатия или распаковки. |
| [DataSource](../../aspose.zip/archiveentry/datasource/) { get; } | Источник записи, если запись была добавлена в архив, а не извлечена. |
| [IsDirectory](../../aspose.zip/archiveentry/isdirectory/) { get; } | Возвращает значение, указывающее, является ли запись каталогом. |
| [ModificationTime](../../aspose.zip/archiveentry/modificationtime/) { get; set; } | Получает или задаёт дату и время последнего изменения. |
| [Name](../../aspose.zip/archiveentry/name/) { get; } | Возвращает имя записи в архиве. |
| [UncompressedSize](../../aspose.zip/archiveentry/uncompressedsize/) { get; } | Возвращает размер оригинального файла. |

## Методы

| Имя | Описание |
| --- | --- |
| [Extract](../../aspose.zip/archiveentry/extract/#extract_1)(Stream, string) | Извлекает запись в предоставленный поток. |
| [Extract](../../aspose.zip/archiveentry/extract/#extract)(string, string) | Извлекает запись в файловую систему по указанному пути. |
| [Open](../../aspose.zip/archiveentry/open/)(string) | Открывает запись для извлечения и предоставляет поток с распакованным содержимым записи. |

## События

| Имя | Описание |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip/archiveentry/compressionprogressed/) | Вызывается, когда часть необработанного потока сжата. |
| event [ExtractionProgressed](../../aspose.zip/archiveentry/extractionprogressed/) | Вызывается, когда часть необработанного потока извлечена. |

## Примечания

Приведите экземпляр `ArchiveEntry` к [`ArchiveEntryEncrypted`](../archiveentryencrypted/), чтобы определить, зашифрована ли запись.

### См. также

* interface [IArchiveFileEntry](../iarchivefileentry/)
* namespace [Aspose.Zip](../../aspose.zip/)
* assembly [Aspose.Zip](../../)


