---
title: "Класс LhaArchive"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Класс Aspose.Zip.Lha.LhaArchive. Этот класс представляет файл архива LHA .lzh"
type: docs
weight: 630
url: /ru/net/aspose.zip.lha/lhaarchive/
---
## LhaArchive class

Этот класс представляет файл архива LHA (.lzh).

```csharp
public class LhaArchive : IArchive
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [LhaArchive](lhaarchive/#constructor)(Stream, LhaLoadOptions) | Инициализирует новый экземпляр класса `LhaArchive` и формирует список записей, которые можно извлечь из архива. |
| [LhaArchive](lhaarchive/#constructor_1)(string, LhaLoadOptions) | Инициализирует новый экземпляр класса `LhaArchive` и формирует список записей, которые можно извлечь из архива. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Entries](../../aspose.zip.lha/lhaarchive/entries/) { get; } | Получает файловые записи типа [`LhaArchiveEntry`](../lhaarchiveentry/), составляющие архив. |

## Методы

| Имя | Описание |
| --- | --- |
| [Dispose](../../aspose.zip.lha/lhaarchive/dispose/)() |  |
| [ExtractToDirectory](../../aspose.zip.lha/lhaarchive/extracttodirectory/)(string) | Извлекает все файлы и каталоги из архива в указанную директорию. |

## Примечания

Поддерживаются только следующие методы сжатия:

**Method**

**Explanation**

**lh0**

Несжатый

**lh4**

8 KiB скользящий словарь и статический Хаффман

**lh5**

16 KiB скользящий словарь и статический Хаффман

**lh6**

64 KiB скользящий словарь и статический Хаффман

**lh7**

128 KiB скользящий словарь и статический Хаффман

**lhx**

1 Mib скользящий словарь и статический Хаффман

**lhd**

Каталог

### См. также

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Lha](../../aspose.zip.lha/)
* assembly [Aspose.Zip](../../)


