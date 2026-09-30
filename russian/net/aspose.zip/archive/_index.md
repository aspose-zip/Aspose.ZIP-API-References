---
title: "Класс Archive"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Класс Aspose.Zip.Archive. Этот класс представляет файл zip‑архива. Используйте его для создания, извлечения или обновления zip‑архивов"
type: docs
weight: 160
url: /ru/net/aspose.zip/archive/
---
## Archive class

Этот класс представляет файл zip‑архива. Используйте его для создания, извлечения или обновления zip‑архивов.

```csharp
public class Archive : IArchive
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [Archive](archive/#constructor)(ArchiveEntrySettings) | Инициализирует новый экземпляр класса `Archive` с необязательными настройками для его записей. |
| [Archive](archive/#constructor_1)(Stream, ArchiveLoadOptions, ArchiveEntrySettings) | Инициализирует новый экземпляр класса `Archive` и формирует список записей, которые можно извлечь из архива. |
| [Archive](archive/#constructor_2)(string, ArchiveLoadOptions, ArchiveEntrySettings) | Инициализирует новый экземпляр класса `Archive` и формирует список записей, которые можно извлечь из архива. |
| [Archive](archive/#constructor_3)(string, string[], ArchiveLoadOptions) | Инициализирует новый экземпляр класса `Archive` из многотомного ZIP‑архива и формирует список записей, которые можно извлечь из архива. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Comment](../../aspose.zip/archive/comment/) { get; } | Получает комментарий к всему архиву. |
| [Entries](../../aspose.zip/archive/entries/) { get; } | Получает записи типа [`ArchiveEntry`](../archiveentry/), составляющие архив. |
| [NewEntrySettings](../../aspose.zip/archive/newentrysettings/) { get; } | Настройки сжатия и шифрования, используемые для недавно добавленных элементов [`ArchiveEntry`](../archiveentry/). |

## Методы

| Имя | Описание |
| --- | --- |
| [CreateEntries](../../aspose.zip/archive/createentries/#createentries)(DirectoryInfo, bool) | Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога. |
| [CreateEntries](../../aspose.zip/archive/createentries/#createentries_1)(string, bool) | Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry)(string, Func&lt;Stream&gt;, ArchiveEntrySettings) | Создаёт одну запись внутри архива. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_2)(string, Stream, ArchiveEntrySettings) | Создаёт одну запись внутри архива. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_1)(string, FileInfo, bool, ArchiveEntrySettings) | Создаёт одну запись внутри архива. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_3)(string, Stream, ArchiveEntrySettings, FileSystemInfo) | Создаёт одну запись внутри архива. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_4)(string, string, bool, ArchiveEntrySettings) | Создаёт одну запись внутри архива. |
| [DeleteEntry](../../aspose.zip/archive/deleteentry/#deleteentry)(ArchiveEntry) | Удаляет первое вхождение указанной записи из списка записей. |
| [DeleteEntry](../../aspose.zip/archive/deleteentry/#deleteentry_1)(int) | Удаляет запись из списка записей по индексу. |
| [Dispose](../../aspose.zip/archive/dispose/)() | Выполняет задачи, определённые приложением, связанные с освобождением, высвобождением или сбросом неуправляемых ресурсов. |
| [ExtractToDirectory](../../aspose.zip/archive/extracttodirectory/)(string) | Извлекает все файлы из архива в указанный каталог. |
| [Save](../../aspose.zip/archive/save/#save)(Stream, ArchiveSaveOptions) | Сохраняет архив в предоставленный поток. |
| [Save](../../aspose.zip/archive/save/#save_1)(string, ArchiveSaveOptions) | Сохраняет архив в указанный файл назначения. |
| [SaveSplit](../../aspose.zip/archive/savesplit/#savesplit)(IVolumeStreamProvider, SplitArchiveSaveOptions) | Сохраняет многотомный архив в потоки, предоставленные поставщиком томов. |
| [SaveSplit](../../aspose.zip/archive/savesplit/#savesplit_1)(string, SplitArchiveSaveOptions) | Сохраняет многотомный архив в указанный каталог назначения. |

### См. также

* interface [IArchive](../iarchive/)
* namespace [Aspose.Zip](../../aspose.zip/)
* assembly [Aspose.Zip](../../)


