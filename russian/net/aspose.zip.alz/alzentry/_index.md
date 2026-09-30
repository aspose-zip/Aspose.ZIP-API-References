---
title: "Класс AlzEntry"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Класс Aspose.Zip.Alz.AlzEntry. Представляет файловую запись в архиве ALZ со всей её метаданной"
type: docs
weight: 30
url: /ru/net/aspose.zip.alz/alzentry/
---
## AlzEntry class

Представляет файловую запись в архиве ALZ со всей её метаданными.

```csharp
public abstract class AlzEntry : IArchiveFileEntry
```

## Свойства

| Имя | Описание |
| --- | --- |
| [CompressedSize](../../aspose.zip.alz/alzentry/compressedsize/) { get; } | Сжатый размер данных файла в байтах. |
| [IsDirectory](../../aspose.zip.alz/alzentry/isdirectory/) { get; } | Возвращает true, если эта запись представляет каталог. |
| [Length](../../aspose.zip.alz/alzentry/length/) { get; } |  |
| [Name](../../aspose.zip.alz/alzentry/name/) { get; } | Имя файла (без пути). |
| [UncompressedSize](../../aspose.zip.alz/alzentry/uncompressedsize/) { get; } | Несжатый размер данных файла в байтах. |

## Методы

| Имя | Описание |
| --- | --- |
| [Extract](../../aspose.zip.alz/alzentry/extract/#extract_1)(Stream, string) | Извлекает запись в предоставленный поток. |
| [Extract](../../aspose.zip.alz/alzentry/extract/#extract)(string, string) | Извлекает запись в файловую систему по указанному пути. |
| [Open](../../aspose.zip.alz/alzentry/open/)(string) | Открывает запись для извлечения и предоставляет поток с распакованным содержимым записи. |

### См. также

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Alz](../../aspose.zip.alz/)
* assembly [Aspose.Zip](../../)


