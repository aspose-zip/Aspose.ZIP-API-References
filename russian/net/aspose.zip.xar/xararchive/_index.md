---
title: "Класс XarArchive"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Aspose.Zip.Xar.XarArchive класс. Этот класс представляет файл архива xar"
type: docs
weight: 1420
url: /ru/net/aspose.zip.xar/xararchive/
---
## XarArchive class

Этот класс представляет файл архива xar.

```csharp
public class XarArchive : IArchive
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [XarArchive](xararchive/#constructor)(XarCompressionSettings) | Инициализирует новый экземпляр класса `XarArchive`. |
| [XarArchive](xararchive/#constructor_1)(Stream, XarLoadOptions) | Инициализирует новый экземпляр класса `XarArchive` и формирует список записей, которые могут быть извлечены из архива. |
| [XarArchive](xararchive/#constructor_2)(string, XarLoadOptions) | Инициализирует новый экземпляр класса `XarArchive` и формирует список записей, которые могут быть извлечены из архива. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Entries](../../aspose.zip.xar/xararchive/entries/) { get; } | Получает записи типа [`XarEntry`](../xarentry/), составляющие архив. |

## Методы

| Имя | Описание |
| --- | --- |
| [CreateEntries](../../aspose.zip.xar/xararchive/createentries/#createentries)(DirectoryInfo, bool, XarCompressionSettings) | Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога. |
| [CreateEntries](../../aspose.zip.xar/xararchive/createentries/#createentries_1)(string, bool, XarCompressionSettings) | Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога. |
| [CreateEntry](../../aspose.zip.xar/xararchive/createentry/#createentry_1)(string, Stream, XarCompressionSettings) | Создаёт одну запись внутри архива. |
| [CreateEntry](../../aspose.zip.xar/xararchive/createentry/#createentry)(string, FileInfo, bool, XarCompressionSettings) | Создаёт одну запись внутри архива. |
| [CreateEntry](../../aspose.zip.xar/xararchive/createentry/#createentry_2)(string, string, bool, XarCompressionSettings) | Создаёт одну запись внутри архива. |
| [DeleteEntry](../../aspose.zip.xar/xararchive/deleteentry/)(XarEntry) | Удаляет первое вхождение конкретной записи из списка записей. |
| [Dispose](../../aspose.zip.xar/xararchive/dispose/)() | Выполняет задачи, определённые приложением, связанные с освобождением, высвобождением или сбросом неуправляемых ресурсов. |
| [ExtractToDirectory](../../aspose.zip.xar/xararchive/extracttodirectory/)(string) | Извлекает все файлы из архива в указанный каталог. |
| [Save](../../aspose.zip.xar/xararchive/save/#save)(Stream, XarSaveOptions) | Сохраняет архив в предоставленный поток. |
| [Save](../../aspose.zip.xar/xararchive/save/#save_1)(string, XarSaveOptions) | Сохраняет архив в указанный файл назначения. |

### См. также

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Xar](../../aspose.zip.xar/)
* assembly [Aspose.Zip](../../)


