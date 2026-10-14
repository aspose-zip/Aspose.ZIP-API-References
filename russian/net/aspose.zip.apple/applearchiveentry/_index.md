---
title: "Класс AppleArchiveEntry"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Aspose.Zip.Apple.AppleArchiveEntry class. Представляет запись файловой системы внутри AppleArchive"
type: docs
weight: 70
url: /ru/net/aspose.zip.apple/applearchiveentry/
---
## AppleArchiveEntry class

Представляет запись файловой системы внутри [`AppleArchive`](../applearchive/).

```csharp
public sealed class AppleArchiveEntry : IArchiveFileEntry
```

## Свойства

| Имя | Описание |
| --- | --- |
| [IsDirectory](../../aspose.zip.apple/applearchiveentry/isdirectory/) { get; } | Возвращает значение, указывающее, является ли запись каталогом. |
| [IsSymbolicLink](../../aspose.zip.apple/applearchiveentry/issymboliclink/) { get; } | Возвращает значение, указывающее, представляет ли запись символическую ссылку. |
| [Length](../../aspose.zip.apple/applearchiveentry/length/) { get; } | Возвращает несжатую длину записи в байтах. |
| [Name](../../aspose.zip.apple/applearchiveentry/name/) { get; } | Возвращает путь к записи внутри архива. |

## Методы

| Имя | Описание |
| --- | --- |
| [Extract](../../aspose.zip.apple/applearchiveentry/extract/#extract_1)(Stream) | Извлекает запись в предоставленный поток. |
| [Extract](../../aspose.zip.apple/applearchiveentry/extract/#extract)(string) | Извлекает запись в файловую систему по указанному пути. |
| [Open](../../aspose.zip.apple/applearchiveentry/open/)() | Открывает запись для извлечения и предоставляет поток с содержимым записи. |

## Примечания

Экземпляр этого класса может представлять обычный файл, каталог или символическую ссылку, полученные из существующего Apple Archive, либо файл или каталог, добавленные в формируемый архив.

### См. также

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Apple](../../aspose.zip.apple/)
* assembly [Aspose.Zip](../../)


