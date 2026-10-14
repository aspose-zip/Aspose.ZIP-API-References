---
title: "SevenZipLZMA2CompressionSettings.SevenZipLZMA2CompressionSettings"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Конструктор SevenZipLZMA2CompressionSettings. Создаёт настройки метода сжатия LZMA2 в архиве 7z."
type: docs
weight: 10
url: /ru/net/aspose.zip.saving/sevenziplzma2compressionsettings/sevenziplzma2compressionsettings/
---
## SevenZipLZMA2CompressionSettings(int) {#constructor}

Создаёт параметры метода сжатия LZMA2 в 7z‑архиве.

```csharp
public SevenZipLZMA2CompressionSettings(int dictionarySize = 16777216)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| dictionarySize | Int32 | Размер буфера истории должен быть в диапазоне от 4096 до 1073741824. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentOutOfRangeException | *dictionarySize* слишком велик или слишком мал. |

## Примечания

Чем больше словарь, тем обычно лучше коэффициент сжатия — но словари, превышающие размер несжатых данных, являются пустой тратой ОЗУ.

### См. также

* class [SevenZipLZMA2CompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../sevenziplzma2compressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## SevenZipLZMA2CompressionSettings(int, int) {#constructor_1}

Создаёт параметры метода сжатия LZMA2 в 7z‑архиве.

```csharp
public SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes = 32)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| dictionarySize | Int32 | Размер буфера истории должен быть в диапазоне от 4096 до 1073741824. |
| fastBytes | Int32 | Контролирует количество быстрых байтов, используемых компрессорами LZMA2. Большее количество быстрых байтов может обеспечить лучшую степень сжатия за счёт скорости сжатия. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentOutOfRangeException | *dictionarySize* слишком большой или слишком маленький, или *fastBytes* слишком большой или слишком маленький. |

## Примечания

Чем больше словарь, тем обычно лучше коэффициент сжатия — но словари, превышающие размер несжатых данных, являются пустой тратой ОЗУ.

### См. также

* class [SevenZipLZMA2CompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../sevenziplzma2compressionsettings/)
* assembly [Aspose.Zip](../../../)


