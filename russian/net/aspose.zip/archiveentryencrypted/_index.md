---
title: "Класс ArchiveEntryEncrypted"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Aspose.Zip.ArchiveEntryEncrypted class. Запись Zip, которую необходимо сжать с шифрованием или распаковать с дешифрованием"
type: docs
weight: 180
url: /ru/net/aspose.zip/archiveentryencrypted/
---
## ArchiveEntryEncrypted class

Запись Zip, которую необходимо сжать с шифрованием или распаковать с дешифрованием.

```csharp
public sealed class ArchiveEntryEncrypted : ArchiveEntry
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Comment](../../aspose.zip/archiveentry/comment/) { get; } | Возвращает комментарий записи в архиве. |
| [CompressedSize](../../aspose.zip/archiveentry/compressedsize/) { get; } | Возвращает размер сжатого файла. |
| [CompressionSettings](../../aspose.zip/archiveentry/compressionsettings/) { get; } | Возвращает настройки сжатия или распаковки. |
| [DataSource](../../aspose.zip/archiveentry/datasource/) { get; } | Источник записи, если запись была добавлена в архив, а не извлечена. |
| [EncryptionSettings](../../aspose.zip/archiveentryencrypted/encryptionsettings/) { get; } | Получает настройки для шифрования или дешифрования. |
| [IsDirectory](../../aspose.zip/archiveentry/isdirectory/) { get; } | Возвращает значение, указывающее, является ли запись каталогом. |
| [ModificationTime](../../aspose.zip/archiveentry/modificationtime/) { get; set; } | Получает или задаёт дату и время последнего изменения. |
| [Name](../../aspose.zip/archiveentry/name/) { get; } | Возвращает имя записи в архиве. |
| [UncompressedSize](../../aspose.zip/archiveentry/uncompressedsize/) { get; } | Возвращает размер оригинального файла. |

## Методы

| Имя | Описание |
| --- | --- |
| [Extract](../../aspose.zip/archiveentry/extract/)(Stream, string) | Извлекает запись в предоставленный поток. |
| [Extract](../../aspose.zip/archiveentry/extract/)(string, string) | Извлекает запись в файловую систему по указанному пути. |
| [Open](../../aspose.zip/archiveentry/open/)(string) | Открывает запись для извлечения и предоставляет поток с распакованным содержимым записи. |

## События

| Имя | Описание |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip/archiveentry/compressionprogressed/) | Вызывается, когда часть необработанного потока сжата. |
| event [ExtractionProgressed](../../aspose.zip/archiveentry/extractionprogressed/) | Вызывается, когда часть необработанного потока извлечена. |

### См. также

* class [ArchiveEntry](../archiveentry/)
* namespace [Aspose.Zip](../../aspose.zip/)
* assembly [Aspose.Zip](../../)


