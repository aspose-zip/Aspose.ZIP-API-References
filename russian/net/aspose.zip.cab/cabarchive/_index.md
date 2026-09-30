---
title: "Класс CabArchive"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Класс Aspose.Zip.Cab.CabArchive. Этот класс представляет файл архива CAB."
type: docs
weight: 310
url: /ru/net/aspose.zip.cab/cabarchive/
---
## CabArchive class

Этот класс представляет файл архива CAB.

```csharp
public class CabArchive : IArchive
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [CabArchive](cabarchive/#constructor)(CabEntrySettings) | Инициализирует новый экземпляр класса `CabArchive`, подготовленный для сжатия. |
| [CabArchive](cabarchive/#constructor_1)(Stream, CabLoadOptions) | Инициализирует новый экземпляр класса `CabArchive` и формирует список записей, которые можно извлечь из архива. |
| [CabArchive](cabarchive/#constructor_2)(string, CabLoadOptions) | Инициализирует новый экземпляр класса `CabArchive` и формирует список записей, которые можно извлечь из архива. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Entries](../../aspose.zip.cab/cabarchive/entries/) { get; } | Получает записи типа [`CabEntry`](../cabentry/), составляющие архив. |

## Методы

| Имя | Описание |
| --- | --- |
| [CreateEntries](../../aspose.zip.cab/cabarchive/createentries/#createentries)(DirectoryInfo, bool) | Добавляет в архив все файлы, рекурсивно, из указанного каталога. |
| [CreateEntries](../../aspose.zip.cab/cabarchive/createentries/#createentries_1)(string, bool) | Добавляет в архив все файлы рекурсивно из указанного пути к каталогу. |
| [CreateEntry](../../aspose.zip.cab/cabarchive/createentry/#createentry_1)(string, FileInfo, CabEntrySettings) | Создаёт одну запись внутри архива. |
| [CreateEntry](../../aspose.zip.cab/cabarchive/createentry/#createentry)(string, Func&lt;Stream&gt;, CabEntrySettings) | Создаёт одну запись внутри архива. |
| [CreateEntry](../../aspose.zip.cab/cabarchive/createentry/#createentry_2)(string, Stream, CabEntrySettings) | Создаёт одну запись внутри архива. |
| [CreateEntry](../../aspose.zip.cab/cabarchive/createentry/#createentry_3)(string, string, CabEntrySettings) | Создаёт одну запись внутри архива. |
| [Dispose](../../aspose.zip.cab/cabarchive/dispose/)() | Выполняет задачи, определённые приложением, связанные с освобождением, высвобождением или сбросом неуправляемых ресурсов. |
| [ExtractToDirectory](../../aspose.zip.cab/cabarchive/extracttodirectory/)(string) | Извлекает все файлы из архива в указанный каталог. |
| [Save](../../aspose.zip.cab/cabarchive/save/#save)(Stream, CabSaveOptions) | Сохраняет архив в предоставленный поток. |
| [Save](../../aspose.zip.cab/cabarchive/save/#save_1)(string, CabSaveOptions) | Сохраняет архив в указанный файл назначения. |

### См. также

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Cab](../../aspose.zip.cab/)
* assembly [Aspose.Zip](../../)


