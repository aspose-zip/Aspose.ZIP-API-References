---
title: "Класс SevenZipArchive"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Aspose.Zip.SevenZip.SevenZipArchive class. Этот класс представляет файл архива 7z. Используйте его для создания и извлечения архивов 7z"
type: docs
weight: 1190
url: /ru/net/aspose.zip.sevenzip/sevenziparchive/
---
## SevenZipArchive class

Этот класс представляет файл архива 7z. Используйте его для создания и извлечения архивов 7z.

```csharp
public class SevenZipArchive : IArchive
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [SevenZipArchive](sevenziparchive/#constructor)(SevenZipEntrySettings) | Инициализирует новый экземпляр класса `SevenZipArchive` с необязательными настройками для его записей. |
| [SevenZipArchive](sevenziparchive/#constructor_1)(Stream, SevenZipLoadOptions) | Инициализирует новый экземпляр класса `SevenZipArchive` и формирует список записей, которые можно извлечь из архива. |
| [SevenZipArchive](sevenziparchive/#constructor_2)(Stream, string) | Инициализирует новый экземпляр класса `SevenZipArchive` и формирует список записей, которые можно извлечь из архива. |
| [SevenZipArchive](sevenziparchive/#constructor_3)(string, SevenZipLoadOptions) | Инициализирует новый экземпляр класса `SevenZipArchive` и формирует список записей, которые можно извлечь из архива. |
| [SevenZipArchive](sevenziparchive/#constructor_4)(string, string) | Инициализирует новый экземпляр класса `SevenZipArchive` и формирует список записей, которые можно извлечь из архива. |
| [SevenZipArchive](sevenziparchive/#constructor_5)(string[], string) | Инициализирует новый экземпляр класса `SevenZipArchive` из многотомного архива 7z и формирует список записей, которые можно извлечь из архива. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Entries](../../aspose.zip.sevenzip/sevenziparchive/entries/) { get; } | Получает записи типа [`SevenZipArchiveEntry`](../sevenziparchiveentry/), составляющие архив. |
| [NewEntrySettings](../../aspose.zip.sevenzip/sevenziparchive/newentrysettings/) { get; } | Настройки сжатия и шифрования, используемые для недавно добавленных элементов [`SevenZipArchiveEntry`](../sevenziparchiveentry/). |

## Методы

| Имя | Описание |
| --- | --- |
| [CreateEntries](../../aspose.zip.sevenzip/sevenziparchive/createentries/#createentries)(DirectoryInfo, bool) | Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога. |
| [CreateEntries](../../aspose.zip.sevenzip/sevenziparchive/createentries/#createentries_1)(string, bool) | Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry)(string, Func&lt;Stream&gt;, SevenZipEntrySettings) | Создаёт одну запись внутри архива. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_2)(string, Stream, SevenZipEntrySettings) | Создаёт одну запись внутри архива. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_1)(string, FileInfo, bool, SevenZipEntrySettings) | Создаёт одну запись внутри архива. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_3)(string, Stream, SevenZipEntrySettings, FileSystemInfo) | Создаёт одну запись внутри архива. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_4)(string, string, bool, SevenZipEntrySettings) | Создаёт одну запись внутри архива. |
| [Dispose](../../aspose.zip.sevenzip/sevenziparchive/dispose/)() | Выполняет задачи, определённые приложением, связанные с освобождением, высвобождением или сбросом неуправляемых ресурсов. |
| [ExtractToDirectory](../../aspose.zip.sevenzip/sevenziparchive/extracttodirectory/)(string, string) | Извлекает все файлы из архива в указанный каталог. |
| [Save](../../aspose.zip.sevenzip/sevenziparchive/save/#save)(Stream, SevenZipArchiveSaveOptions) | Сохраняет архив 7z в предоставленный поток. |
| [Save](../../aspose.zip.sevenzip/sevenziparchive/save/#save_1)(string, SevenZipArchiveSaveOptions) | Сохраняет архив в указанный файл назначения. |
| [SaveSplit](../../aspose.zip.sevenzip/sevenziparchive/savesplit/)(string, SplitSevenZipArchiveSaveOptions) | Сохраняет многотомный архив в указанный каталог назначения. |

### См. также

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.SevenZip](../../aspose.zip.sevenzip/)
* assembly [Aspose.Zip](../../)


