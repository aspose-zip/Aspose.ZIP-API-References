---
title: "Класс RarArchiveEntryPlain"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Класс Aspose.Zip.Rar.RarArchiveEntryPlain. Запись Rar, которую необходимо распаковать без расшифровки"
type: docs
weight: 820
url: /ru/net/aspose.zip.rar/rararchiveentryplain/
---
## RarArchiveEntryPlain class

Запись Rar, которую необходимо распаковать без расшифровки.

```csharp
public sealed class RarArchiveEntryPlain : RarArchiveEntry
```

## Свойства

| Имя | Описание |
| --- | --- |
| [CompressedSize](../../aspose.zip.rar/rararchiveentry/compressedsize/) { get; } | Получает размер сжатого файла. |
| [CreationTime](../../aspose.zip.rar/rararchiveentry/creationtime/) { get; } | Получает дату и время создания. |
| [IsDirectory](../../aspose.zip.rar/rararchiveentry/isdirectory/) { get; } | Возвращает значение, указывающее, является ли запись каталогом. |
| [LastAccessTime](../../aspose.zip.rar/rararchiveentry/lastaccesstime/) { get; } | Получает дату и время последнего доступа. |
| [ModificationTime](../../aspose.zip.rar/rararchiveentry/modificationtime/) { get; } | Получает дату и время последнего изменения. |
| [Name](../../aspose.zip.rar/rararchiveentry/name/) { get; } | Возвращает имя записи в архиве. |
| [UncompressedSize](../../aspose.zip.rar/rararchiveentry/uncompressedsize/) { get; } | Получает размер оригинального файла. |

## Методы

| Имя | Описание |
| --- | --- |
| [Extract](../../aspose.zip.rar/rararchiveentry/extract/)(Stream, string) | Извлекает запись в предоставленный поток. |
| [Extract](../../aspose.zip.rar/rararchiveentry/extract/)(string, string) | Извлекает запись в файловую систему по указанному пути. |
| [Open](../../aspose.zip.rar/rararchiveentry/open/)(string) | Открывает запись для извлечения и предоставляет поток с распакованным содержимым записи. |

## События

| Имя | Описание |
| --- | --- |
| event [ExtractionProgressed](../../aspose.zip.rar/rararchiveentry/extractionprogressed/) | Вызывается, когда часть необработанного потока извлечена. |

### См. также

* class [RarArchiveEntry](../rararchiveentry/)
* namespace [Aspose.Zip.Rar](../../aspose.zip.rar/)
* assembly [Aspose.Zip](../../)


