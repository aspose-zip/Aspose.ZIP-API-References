---
title: "Класс EggEntry"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Класс Aspose.Zip.Egg.EggEntry. Представляет файловую запись в EGG‑архиве со всей её метаданными"
type: docs
weight: 470
url: /ru/net/aspose.zip.egg/eggentry/
---
## EggEntry class

Представляет запись файла в архиве EGG со всей его метаданными.

```csharp
public abstract class EggEntry : IArchiveFileEntry
```

## Свойства

| Имя | Описание |
| --- | --- |
| [CompressedSize](../../aspose.zip.egg/eggentry/compressedsize/) { get; } | Получает сжатый размер записи. |
| [IsDirectory](../../aspose.zip.egg/eggentry/isdirectory/) { get; } | Получает значение, указывающее, является ли эта запись каталогом. |
| [Length](../../aspose.zip.egg/eggentry/length/) { get; } |  |
| [ModificationTime](../../aspose.zip.egg/eggentry/modificationtime/) { get; } | Получает или задаёт дату и время последнего изменения. |
| [Name](../../aspose.zip.egg/eggentry/name/) { get; } | Получает имя записи в архиве. |
| [UncompressedSize](../../aspose.zip.egg/eggentry/uncompressedsize/) { get; } | Получает несжатый размер записи. |

## Методы

| Имя | Описание |
| --- | --- |
| [Extract](../../aspose.zip.egg/eggentry/extract/#extract_1)(Stream) | Извлекает запись в предоставленный поток. |
| [Extract](../../aspose.zip.egg/eggentry/extract/#extract)(string) | Извлекает запись в файловую систему по указанному пути. |
| [Open](../../aspose.zip.egg/eggentry/open/)() | Открывает запись для извлечения и предоставляет поток с распакованным содержимым записи. |

### См. также

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Egg](../../aspose.zip.egg/)
* assembly [Aspose.Zip](../../)


