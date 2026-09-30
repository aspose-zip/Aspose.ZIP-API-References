---
title: "XzArchiveSettings.XzArchiveSettings"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Конструктор XzArchiveSettings. Инициализирует новый экземпляр класса XzArchiveSettings, используя одиночное сжатие LZMA2."
type: docs
weight: 10
url: /ru/net/aspose.zip.xz.settings/xzarchivesettings/xzarchivesettings/
---
## XzArchiveSettings() {#constructor}

Инициализирует новый экземпляр класса [`XzArchiveSettings`](../), используя одиночное сжатие LZMA2.

```csharp
public XzArchiveSettings()
```

## Примечания

Размер словаря по умолчанию в фильтре LZMA2 равен 16 мегабайтам, размер блока по умолчанию — 64 мегабайта, тип контрольной суммы по умолчанию — CRC32.

### См. также

* class [XzArchiveSettings](../)
* namespace [Aspose.Zip.Xz.Settings](../../xzarchivesettings/)
* assembly [Aspose.Zip](../../../)

---

## XzArchiveSettings(XzFilterSettings[], long, XzCheckType) {#constructor_1}

Инициализирует новый экземпляр класса [`XzArchiveSettings`](../) с пользовательскими параметрами.

```csharp
public XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| filters | XzFilterSettings[] | Фильтры (компрессоры), которые последовательно применяются для создания [`XzArchive`](../../../aspose.zip.xz/xzarchive/). Это может быть один [`XzLZMA2FilterSettings`](../../xzlzma2filtersettings/) или пара [`XzBcjX86FilterSettings`](../../xzbcjx86filtersettings/) и [`XzLZMA2FilterSettings`](../../xzlzma2filtersettings/). |
| blockSize | Int64 | Размер блока xz-архива. |
| checkType | XzCheckType | Тип вычисления контрольной суммы для несжатых данных. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentOutOfRangeException | *blockSize* отрицателен. |
| ArgumentNullException | *filters* равен null |
| ArgumentException | *filters* содержит менее одного или более двух фильтров, либо последний фильтр не является [`XzLZMA2FilterSettings`](../../xzlzma2filtersettings/). |

## Примеры

```csharp
using (FileStream xzFile = File.Open("archive.xz", FileMode.Create))
{
    XzLZMA2FilterSettings filter = new XzLZMA2FilterSettings(5242880);
    XzArchiveSettings settings = new XzArchiveSettings(new XzFilterSettings[] {filter}, 10485760, XzCheckType.Crc32);
    using (var archive = new XzArchive(settings))
    {
        archive.SetSource("data.bin");
        archive.Save(xzFile);
     }
}
```

### См. также

* class [XzFilterSettings](../../xzfiltersettings/)
* enum [XzCheckType](../../xzchecktype/)
* class [XzArchiveSettings](../)
* namespace [Aspose.Zip.Xz.Settings](../../xzarchivesettings/)
* assembly [Aspose.Zip](../../../)


