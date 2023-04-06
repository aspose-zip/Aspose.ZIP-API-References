---
title: Class CpioArchive
second_title: Aspose.ZIP для справочника API .NET
description: Aspose.Zip.Cpio.CpioArchive сорт. Этот класс представляет файл архива cpio.
type: docs
weight: 160
url: /ru/net/aspose.zip.cpio/cpioarchive/
---
## CpioArchive class

Этот класс представляет файл архива cpio.

```csharp
public class CpioArchive : IArchive
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [CpioArchive](cpioarchive/#constructor)() | Инициализирует новый экземпляр`CpioArchive` класс. |
| [CpioArchive](cpioarchive/#constructor_1)(Stream) | Инициализирует новый экземпляр`CpioArchive` список записей классов и композиций можно извлечь из архива. |
| [CpioArchive](cpioarchive/#constructor_2)(string) | Инициализирует новый экземпляр`CpioArchive` список записей классов и композиций можно извлечь из архива. |

## Характеристики

| Имя | Описание |
| --- | --- |
| [Entries](../../aspose.zip.cpio/cpioarchive/entries/) { get; } | Получает записи[`CpioEntry`](../cpioentry/) тип составляющий архив. |

## Методы

| Имя | Описание |
| --- | --- |
| [CreateEntries](../../aspose.zip.cpio/cpioarchive/createentries/#createentries)(DirectoryInfo, bool) | Добавляет в архив все файлы и каталоги рекурсивно в заданном каталоге. |
| [CreateEntries](../../aspose.zip.cpio/cpioarchive/createentries/#createentries_1)(string, bool) | Добавляет в архив все файлы и каталоги рекурсивно в заданном каталоге. |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry_1)(string, Stream) | Создать одну запись в архиве. |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry)(string, FileInfo, bool) | Создать одну запись в архиве. |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry_2)(string, string, bool) | Создать одну запись в архиве. |
| [DeleteEntry](../../aspose.zip.cpio/cpioarchive/deleteentry/#deleteentry)(CpioEntry) | Удаляет первое вхождение определенной записи из списка записей. |
| [DeleteEntry](../../aspose.zip.cpio/cpioarchive/deleteentry/#deleteentry_1)(int) | Удаляет запись из списка записей по индексу. |
| [Dispose](../../aspose.zip.cpio/cpioarchive/dispose/)() | Выполняет определяемые приложением задачи, связанные с освобождением, высвобождением или сбросом неуправляемых ресурсов. |
| [ExtractToDirectory](../../aspose.zip.cpio/cpioarchive/extracttodirectory/)(string) | Извлекает все файлы из архива в указанный каталог. |
| [Save](../../aspose.zip.cpio/cpioarchive/save/#save)(Stream, CpioFormat) | Сохраняет архив в указанный поток. |
| [Save](../../aspose.zip.cpio/cpioarchive/save/#save_1)(string, CpioFormat) | Сохраняет архив в указанный файл назначения. |
| [SaveGzipped](../../aspose.zip.cpio/cpioarchive/savegzipped/#savegzipped)(Stream, CpioFormat) | Сохраняет архив в поток со сжатием gzip. |
| [SaveGzipped](../../aspose.zip.cpio/cpioarchive/savegzipped/#savegzipped_1)(string, CpioFormat) | Сохраняет архив в файл по пути со сжатием gzip. |
| [SaveXzCompressed](../../aspose.zip.cpio/cpioarchive/savexzcompressed/#savexzcompressed)(Stream, CpioFormat, XzArchiveSettings) | Сохраняет архив в поток со сжатием xz. |
| [SaveXzCompressed](../../aspose.zip.cpio/cpioarchive/savexzcompressed/#savexzcompressed_1)(string, CpioFormat, XzArchiveSettings) | Сохраняет архив в путь по пути со сжатием xz. |

### Смотрите также

* interface [IArchive](../../aspose.zip/iarchive/)
* пространство имен [Aspose.Zip.Cpio](../../aspose.zip.cpio/)
* сборка [Aspose.Zip](../../)


