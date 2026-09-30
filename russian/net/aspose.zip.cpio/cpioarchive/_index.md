---
title: "Класс CpioArchive"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Класс Aspose.Zip.Cpio.CpioArchive. Этот класс представляет файл архива cpio"
type: docs
weight: 410
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
| [CpioArchive](cpioarchive/#constructor)() | Инициализирует новый экземпляр класса `CpioArchive`. |
| [CpioArchive](cpioarchive/#constructor_1)(Stream) | Инициализирует новый экземпляр класса `CpioArchive` и формирует список записей, которые можно извлечь из архива. |
| [CpioArchive](cpioarchive/#constructor_2)(string) | Инициализирует новый экземпляр класса `CpioArchive` и формирует список записей, которые можно извлечь из архива. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Entries](../../aspose.zip.cpio/cpioarchive/entries/) { get; } | Получает записи типа [`CpioEntry`](../cpioentry/), составляющие архив. |

## Методы

| Имя | Описание |
| --- | --- |
| [CreateEntries](../../aspose.zip.cpio/cpioarchive/createentries/#createentries)(DirectoryInfo, bool) | Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога. |
| [CreateEntries](../../aspose.zip.cpio/cpioarchive/createentries/#createentries_1)(string, bool) | Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога. |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry_1)(string, Stream) | Создаёт одну запись внутри архива. |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry)(string, FileInfo, bool) | Создаёт одну запись внутри архива. |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry_2)(string, string, bool) | Создаёт одну запись внутри архива. |
| [DeleteEntry](../../aspose.zip.cpio/cpioarchive/deleteentry/#deleteentry)(CpioEntry) | Удаляет первое вхождение конкретной записи из списка записей. |
| [DeleteEntry](../../aspose.zip.cpio/cpioarchive/deleteentry/#deleteentry_1)(int) | Удаляет запись из списка записей по индексу. |
| [Dispose](../../aspose.zip.cpio/cpioarchive/dispose/)() | Выполняет задачи, определённые приложением, связанные с освобождением, высвобождением или сбросом неуправляемых ресурсов. |
| [ExtractToDirectory](../../aspose.zip.cpio/cpioarchive/extracttodirectory/)(string) | Извлекает все файлы из архива в указанный каталог. |
| [Save](../../aspose.zip.cpio/cpioarchive/save/#save)(Stream, CpioFormat) | Сохраняет архив в предоставленный поток. |
| [Save](../../aspose.zip.cpio/cpioarchive/save/#save_1)(string, CpioFormat) | Сохраняет архив в указанный файл назначения. |
| [SaveGzipped](../../aspose.zip.cpio/cpioarchive/savegzipped/#savegzipped)(Stream, CpioFormat) | Сохраняет архив в поток с gzip‑сжатием. |
| [SaveGzipped](../../aspose.zip.cpio/cpioarchive/savegzipped/#savegzipped_1)(string, CpioFormat) | Сохраняет архив в файл по пути с gzip‑сжатием. |
| [SaveLzipped](../../aspose.zip.cpio/cpioarchive/savelzipped/#savelzipped)(Stream, CpioFormat) | Сохраняет архив в поток с lzip‑сжатием. |
| [SaveLzipped](../../aspose.zip.cpio/cpioarchive/savelzipped/#savelzipped_1)(string, CpioFormat) | Сохраняет архив в файл по пути с lzip‑сжатием. |
| [SaveLZMACompressed](../../aspose.zip.cpio/cpioarchive/savelzmacompressed/#savelzmacompressed)(Stream, CpioFormat) | Сохраняет архив в поток с компрессией LZMA. |
| [SaveLZMACompressed](../../aspose.zip.cpio/cpioarchive/savelzmacompressed/#savelzmacompressed_1)(string, CpioFormat) | Сохраняет архив в файл по пути с компрессией lzma. |
| [SaveXzCompressed](../../aspose.zip.cpio/cpioarchive/savexzcompressed/#savexzcompressed)(Stream, CpioFormat, XzArchiveSettings) | Сохраняет архив в поток с xz‑сжатием. |
| [SaveXzCompressed](../../aspose.zip.cpio/cpioarchive/savexzcompressed/#savexzcompressed_1)(string, CpioFormat, XzArchiveSettings) | Сохраняет архив по указанному пути с xz‑сжатием. |
| [SaveZCompressed](../../aspose.zip.cpio/cpioarchive/savezcompressed/#savezcompressed)(Stream, CpioFormat) | Сохраняет архив в поток с Z‑сжатием. |
| [SaveZCompressed](../../aspose.zip.cpio/cpioarchive/savezcompressed/#savezcompressed_1)(string, CpioFormat) | Сохраняет архив по указанному пути с Z‑сжатием |
| [SaveZstandard](../../aspose.zip.cpio/cpioarchive/savezstandard/#savezstandard)(Stream, CpioFormat) | Сохраняет архив в поток с компрессией Zstandard. |
| [SaveZstandard](../../aspose.zip.cpio/cpioarchive/savezstandard/#savezstandard_1)(string, CpioFormat) | Сохраняет архив в файл по пути с компрессией Zstandard. |

### См. также

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Cpio](../../aspose.zip.cpio/)
* assembly [Aspose.Zip](../../)


