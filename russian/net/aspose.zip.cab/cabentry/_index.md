---
title: "Класс CabEntry"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Класс Aspose.Zip.Cab.CabEntry. Представляет отдельный файл внутри CAB-архива."
type: docs
weight: 330
url: /ru/net/aspose.zip.cab/cabentry/
---
## CabEntry class

Представляет отдельный файл внутри архива CAB.

```csharp
public sealed class CabEntry : IArchiveFileEntry
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Length](../../aspose.zip.cab/cabentry/length/) { get; } | Получает длину записи в байтах. |
| [ModificationTime](../../aspose.zip.cab/cabentry/modificationtime/) { get; } | Получает дату и время последнего изменения. |
| [Name](../../aspose.zip.cab/cabentry/name/) { get; } | Возвращает имя записи в архиве. |

## Методы

| Имя | Описание |
| --- | --- |
| [Extract](../../aspose.zip.cab/cabentry/extract/#extract_1)(Stream) | Извлекает запись в предоставленный поток. |
| [Extract](../../aspose.zip.cab/cabentry/extract/#extract)(string) | Извлекает запись в файловую систему по указанному пути. |
| [Open](../../aspose.zip.cab/cabentry/open/)() | Открывает запись для извлечения и предоставляет поток с содержимым записи. |
| override [ToString](../../aspose.zip.cab/cabentry/tostring/)() |  |

### См. также

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Cab](../../aspose.zip.cab/)
* assembly [Aspose.Zip](../../)


