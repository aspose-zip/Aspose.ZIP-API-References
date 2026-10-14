---
title: "Класс IsoArchive"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Класс Aspose.Zip.Iso.IsoArchive. Представляет ISO‑архив ISO 9660"
type: docs
weight: 570
url: /ru/net/aspose.zip.iso/isoarchive/
---
## IsoArchive class

Представляет ISO‑архив (ISO 9660).

```csharp
public sealed class IsoArchive : IArchive
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [IsoArchive](isoarchive/#constructor)() | Инициализирует новый экземпляр класса `IsoArchive` и создает пустой ISO‑архив для добавления новых файлов и каталогов. |
| [IsoArchive](isoarchive/#constructor_1)(Stream, IsoLoadOptions) | Инициализирует новый экземпляр класса `IsoArchive` и формирует список записей, которые могут быть извлечены из архива. |
| [IsoArchive](isoarchive/#constructor_2)(string, IsoLoadOptions) | Инициализирует новый экземпляр класса `IsoArchive` и формирует список записей, которые могут быть извлечены из архива. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Entries](../../aspose.zip.iso/isoarchive/entries/) { get; } | Получает записи типа [`IsoEntry`](../isoentry/), составляющие архив. |

## Методы

| Имя | Описание |
| --- | --- |
| [CreateDirectory](../../aspose.zip.iso/isoarchive/createdirectory/)(string) | Добавляет каталог в ISO‑образ. |
| [CreateEntry](../../aspose.zip.iso/isoarchive/createentry/#createentry)(string) | Добавляет файл в ISO‑образ. |
| [CreateEntry](../../aspose.zip.iso/isoarchive/createentry/#createentry_1)(string, Stream) | Добавляет файл в ISO‑образ. |
| [CreateEntry](../../aspose.zip.iso/isoarchive/createentry/#createentry_2)(string, string) | Добавляет файл в ISO‑образ. |
| [Dispose](../../aspose.zip.iso/isoarchive/dispose/)() | Выполняет задачи, определённые приложением, связанные с освобождением, высвобождением или сбросом неуправляемых ресурсов. |
| [ExtractToDirectory](../../aspose.zip.iso/isoarchive/extracttodirectory/)(string) | Извлекает все записи в указанный каталог. |
| [Save](../../aspose.zip.iso/isoarchive/save/#save)(Stream, IsoSaveOptions) | Сохраняет ISO‑образ в указанный поток. |
| [Save](../../aspose.zip.iso/isoarchive/save/#save_1)(string, IsoSaveOptions) | Сохраняет ISO‑образ по указанному пути. |

### См. также

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Iso](../../aspose.zip.iso/)
* assembly [Aspose.Zip](../../)


