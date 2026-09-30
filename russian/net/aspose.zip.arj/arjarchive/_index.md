---
title: "Класс ArjArchive"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Класс Aspose.Zip.Arj.ArjArchive. Этот класс представляет файл ARJ-архива"
type: docs
weight: 250
url: /ru/net/aspose.zip.arj/arjarchive/
---
## ArjArchive class

Этот класс представляет файл архива ARJ.

```csharp
public class ArjArchive : IArchive
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [ArjArchive](arjarchive/#constructor)(Stream, ArjLoadOptions) | Инициализирует новый экземпляр класса `ArjArchive` и формирует список записей, которые можно извлечь из архива. |
| [ArjArchive](arjarchive/#constructor_1)(string, ArjLoadOptions) | Инициализирует новый экземпляр класса `ArjArchive` и формирует список записей, которые можно извлечь из архива. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Commentary](../../aspose.zip.arj/arjarchive/commentary/) { get; } | Получает комментарий. |
| [Entries](../../aspose.zip.arj/arjarchive/entries/) { get; } | Получает записи типа [`ArjEntryPlain`](../arjentryplain/), составляющие ARJ-архив. |
| [Name](../../aspose.zip.arj/arjarchive/name/) { get; } | Получает оригинальное имя. |

## Методы

| Имя | Описание |
| --- | --- |
| [Dispose](../../aspose.zip.arj/arjarchive/dispose/)() | Выполняет задачи, определённые приложением, связанные с освобождением, высвобождением или сбросом неуправляемых ресурсов. |
| [ExtractToDirectory](../../aspose.zip.arj/arjarchive/extracttodirectory/)(string) | Извлекает все записи в указанный каталог. |

## Примечания

Поддерживаются только следующие методы сжатия:

**Method**

**Explanation**

**0**

Несжатый

**1**

Комбинация LZ77 и адаптивного кодирования Хаффмана. Лучшее соотношение.

**2**

Комбинация LZ77 и адаптивного кодирования Хаффмана.

**3**

Комбинация LZ77 и адаптивного кодирования Хаффмана. Наивысшая скорость.

### См. также

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Arj](../../aspose.zip.arj/)
* assembly [Aspose.Zip](../../)


