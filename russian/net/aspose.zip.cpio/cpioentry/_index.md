---
title: "Класс CpioEntry"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Класс Aspose.Zip.Cpio.CpioEntry. Представляет отдельный файл в архиве cpio"
type: docs
weight: 420
url: /ru/net/aspose.zip.cpio/cpioentry/
---
## CpioEntry class

Представляет отдельный файл внутри архива cpio.

```csharp
public sealed class CpioEntry : IArchiveFileEntry
```

## Свойства

| Имя | Описание |
| --- | --- |
| [IsDirectory](../../aspose.zip.cpio/cpioentry/isdirectory/) { get; } | Возвращает значение, указывающее, является ли запись каталогом. |
| [LastWriteTimeUtc](../../aspose.zip.cpio/cpioentry/lastwritetimeutc/) { get; } | Получает время последней записи. |
| [Length](../../aspose.zip.cpio/cpioentry/length/) { get; } | Получает длину записи в байтах. |
| [Name](../../aspose.zip.cpio/cpioentry/name/) { get; } | Возвращает имя записи в архиве. |
| [Parent](../../aspose.zip.cpio/cpioentry/parent/) { get; } | Получает архив, к которому принадлежит запись. |

## Методы

| Имя | Описание |
| --- | --- |
| [Extract](../../aspose.zip.cpio/cpioentry/extract/#extract_1)(Stream) | Извлекает запись в предоставленный поток. |
| [Extract](../../aspose.zip.cpio/cpioentry/extract/#extract)(string) | Извлекает запись в файловую систему по указанному пути. |
| [Open](../../aspose.zip.cpio/cpioentry/open/)() | Открывает запись для извлечения и предоставляет поток с содержимым записи. |
| override [ToString](../../aspose.zip.cpio/cpioentry/tostring/)() |  |

### См. также

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Cpio](../../aspose.zip.cpio/)
* assembly [Aspose.Zip](../../)


