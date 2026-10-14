---
title: "Класс WimArchive"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Класс Aspose.Zip.Wim.WimArchive. Этот класс представляет файл архива wim."
type: docs
weight: 1330
url: /ru/net/aspose.zip.wim/wimarchive/
---
## WimArchive class

Этот класс представляет файл архива wim.

```csharp
public class WimArchive : IArchive
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [WimArchive](wimarchive/#constructor)(Stream, WimLoadOptions) | Инициализирует новый экземпляр класса `WimArchive` и формирует список записей, которые можно извлечь из архива. |
| [WimArchive](wimarchive/#constructor_1)(string, WimLoadOptions) | Инициализирует новый экземпляр класса `WimArchive` и формирует список записей, которые можно извлечь из архива. |

## Свойства

| Имя | Описание |
| --- | --- |
| [BootImageIndex](../../aspose.zip.wim/wimarchive/bootimageindex/) { get; } | Получает (нумерацию с нуля) индекс загрузочного образа. |
| [Entries](../../aspose.zip.wim/wimarchive/entries/) { get; } | Получает записи типа [`WimEntry`](../wimentry/), составляющие архив. |
| [FileFormatVersion](../../aspose.zip.wim/wimarchive/fileformatversion/) { get; } | Получает версию формата файла. |
| [Guid](../../aspose.zip.wim/wimarchive/guid/) { get; } | Получает идентифицирующий GUID архива. |
| [Images](../../aspose.zip.wim/wimarchive/images/) { get; } | Получает записи типа [`WimImage`](../wimimage/), составляющие архив. |
| [Manifest](../../aspose.zip.wim/wimarchive/manifest/) { get; } | Получает встроенный манифест, описывающий файл и содержащиеся образы. |

## Методы

| Имя | Описание |
| --- | --- |
| [Dispose](../../aspose.zip.wim/wimarchive/dispose/)() | Выполняет задачи, определённые приложением, связанные с освобождением, высвобождением или сбросом неуправляемых ресурсов. |
| [ExtractToDirectory](../../aspose.zip.wim/wimarchive/extracttodirectory/)(string) | Извлекает архив в файл по указанному пути. |

### См. также

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Wim](../../aspose.zip.wim/)
* assembly [Aspose.Zip](../../)


