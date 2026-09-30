---
title: "Класс AppleArchive"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Aspose.Zip.Apple.AppleArchive class. Этот класс представляет файл Apple Archive .aar. Используйте его для создания файлов Apple Archive"
type: docs
weight: 60
url: /ru/net/aspose.zip.apple/applearchive/
---
## AppleArchive class

Этот класс представляет файл Apple Archive (.aar). Используйте его для создания файлов Apple Archive.

```csharp
public class AppleArchive : IArchive
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [AppleArchive](applearchive/#constructor)(AppleArchiveEntrySettings) | Инициализирует новый экземпляр класса `AppleArchive` с настройками, используемыми для составленных записей. |
| [AppleArchive](applearchive/#constructor_1)(Stream, AppleArchiveLoadOptions) | Инициализирует новый экземпляр класса `AppleArchive` и создает список записей, который может быть извлечен из архива. |
| [AppleArchive](applearchive/#constructor_2)(string, AppleArchiveLoadOptions) | Инициализирует новый экземпляр класса `AppleArchive` и создает список записей, который может быть извлечен из архива. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Entries](../../aspose.zip.apple/applearchive/entries/) { get; } | Получает записи, составляющие архив. |
| [IsSolid](../../aspose.zip.apple/applearchive/issolid/) { get; } | Получает значение, указывающее, использует ли архив сплошное сжатие. В сплошном режиме все данные записей сжаты в один поток, и отдельное извлечение записей недоступно. Вместо этого используйте [`ExtractToDirectory`](../../aspose.zip/iarchive/extracttodirectory/). |
| [NewEntrySettings](../../aspose.zip.apple/applearchive/newentrysettings/) { get; } | Получает настройки, используемые для новых составленных записей. |

## Методы

| Имя | Описание |
| --- | --- |
| [CreateEntries](../../aspose.zip.apple/applearchive/createentries/)(DirectoryInfo, bool) | Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога. |
| [CreateEntry](../../aspose.zip.apple/applearchive/createentry/#createentry_1)(string, Stream) | Создает одну запись в архиве. |
| [CreateEntry](../../aspose.zip.apple/applearchive/createentry/#createentry)(string, FileInfo, bool) | Создает одну запись в архиве. |
| [CreateEntry](../../aspose.zip.apple/applearchive/createentry/#createentry_2)(string, string, bool) | Создает одну запись в архиве. |
| [Dispose](../../aspose.zip.apple/applearchive/dispose/)() | Выполняет задачи, определённые приложением, связанные с освобождением, высвобождением или сбросом неуправляемых ресурсов. |
| [ExtractToDirectory](../../aspose.zip.apple/applearchive/extracttodirectory/)(string) | Извлекает все файлы из архива в указанный каталог. |
| [Save](../../aspose.zip.apple/applearchive/save/#save)(Stream) | Сохраняет архив в предоставленный поток. |
| [Save](../../aspose.zip.apple/applearchive/save/#save_1)(string) | Сохраняет архив в указанный файл назначения. |

## Примечания

Apple и Apple Archive являются товарными знаками компании Apple Inc.

### См. также

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Apple](../../aspose.zip.apple/)
* assembly [Aspose.Zip](../../)


