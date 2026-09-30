---
title: "Класс SharArchive"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Класс Aspose.Zip.Shar.SharArchive. Этот класс представляет файл архива shar."
type: docs
weight: 1240
url: /ru/net/aspose.zip.shar/shararchive/
---
## SharArchive class

Этот класс представляет файл архива shar.

```csharp
public class SharArchive : IDisposable
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [SharArchive](shararchive/#constructor)() | Инициализирует новый экземпляр класса `SharArchive`. |
| [SharArchive](shararchive/#constructor_1)(string) | Инициализирует новый экземпляр класса `SharArchive`, подготовленный для распаковки. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Entries](../../aspose.zip.shar/shararchive/entries/) { get; } | Получает записи типа [`SharEntry`](../sharentry/), составляющие архив. |

## Методы

| Имя | Описание |
| --- | --- |
| [CreateEntries](../../aspose.zip.shar/shararchive/createentries/#createentries)(DirectoryInfo, bool) | Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога. |
| [CreateEntries](../../aspose.zip.shar/shararchive/createentries/#createentries_1)(string, bool) | Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога. |
| [CreateEntry](../../aspose.zip.shar/shararchive/createentry/#createentry_1)(string, Stream) | Создаёт одну запись внутри архива. |
| [CreateEntry](../../aspose.zip.shar/shararchive/createentry/#createentry)(string, FileInfo, bool) | Создаёт одну запись внутри архива. |
| [CreateEntry](../../aspose.zip.shar/shararchive/createentry/#createentry_2)(string, string, bool) | Создаёт одну запись внутри архива. |
| [DeleteEntry](../../aspose.zip.shar/shararchive/deleteentry/#deleteentry_1)(int) | Удаляет запись из списка записей по индексу. |
| [DeleteEntry](../../aspose.zip.shar/shararchive/deleteentry/#deleteentry)(SharEntry) | Удаляет первое вхождение конкретной записи из списка записей. |
| [Dispose](../../aspose.zip.shar/shararchive/dispose/)() | Выполняет задачи, определённые приложением, связанные с освобождением, высвобождением или сбросом неуправляемых ресурсов. |
| [Save](../../aspose.zip.shar/shararchive/save/#save)(Stream) | Сохраняет архив в предоставленный поток. |
| [Save](../../aspose.zip.shar/shararchive/save/#save_1)(string) | Сохраняет архив в указанный файл назначения. |

### См. также

* namespace [Aspose.Zip.Shar](../../aspose.zip.shar/)
* assembly [Aspose.Zip](../../)


