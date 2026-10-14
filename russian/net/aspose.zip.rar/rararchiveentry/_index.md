---
title: "Класс RarArchiveEntry"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Класс Aspose.Zip.Rar.RarArchiveEntry. Представляет отдельный файл в архиве"
type: docs
weight: 800
url: /ru/net/aspose.zip.rar/rararchiveentry/
---
## RarArchiveEntry class

Представляет отдельный файл в архиве.

```csharp
public abstract class RarArchiveEntry : IArchiveFileEntry
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
| [Extract](../../aspose.zip.rar/rararchiveentry/extract/#extract_1)(Stream, string) | Извлекает запись в предоставленный поток. |
| [Extract](../../aspose.zip.rar/rararchiveentry/extract/#extract)(string, string) | Извлекает запись в файловую систему по указанному пути. |
| [Open](../../aspose.zip.rar/rararchiveentry/open/)(string) | Открывает запись для извлечения и предоставляет поток с распакованным содержимым записи. |

## События

| Имя | Описание |
| --- | --- |
| event [ExtractionProgressed](../../aspose.zip.rar/rararchiveentry/extractionprogressed/) | Вызывается, когда часть необработанного потока извлечена. |

## Примечания

Преобразуйте экземпляр `RarArchiveEntry` к [`RarArchiveEntryEncrypted`](../rararchiveentryencrypted/), чтобы определить, зашифрована ли запись.

### См. также

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Rar](../../aspose.zip.rar/)
* assembly [Aspose.Zip](../../)


