---
title: "Класс AlzEntryEncrypted"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Класс Aspose.Zip.Alz.AlzEntryEncrypted. Запись ALZ, которую необходимо расшифровать перед распаковкой"
type: docs
weight: 40
url: /ru/net/aspose.zip.alz/alzentryencrypted/
---
## AlzEntryEncrypted class

Запись ALZ, которую необходимо расшифровать перед распаковкой.

```csharp
public sealed class AlzEntryEncrypted : AlzEntry
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
| [Extract](../../aspose.zip.alz/alzentry/extract/)(Stream, string) | Извлекает запись в предоставленный поток. |
| [Extract](../../aspose.zip.alz/alzentry/extract/)(string, string) | Извлекает запись в файловую систему по указанному пути. |
| [Open](../../aspose.zip.alz/alzentry/open/)(string) | Открывает запись для извлечения и предоставляет поток с распакованным содержимым записи. |

### См. также

* class [AlzEntry](../alzentry/)
* namespace [Aspose.Zip.Alz](../../aspose.zip.alz/)
* assembly [Aspose.Zip](../../)


