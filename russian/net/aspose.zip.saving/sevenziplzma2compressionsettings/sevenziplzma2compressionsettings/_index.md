---
title: SevenZipLZMA2CompressionSettings.SevenZipLZMA2CompressionSettings
second_title: Aspose.ZIP для справочника API .NET
description: SevenZipLZMA2CompressionSettings строитель. Задает настройки для метода сжатия LZMA2 в архиве 7z.
type: docs
weight: 10
url: /ru/net/aspose.zip.saving/sevenziplzma2compressionsettings/sevenziplzma2compressionsettings/
---
## SevenZipLZMA2CompressionSettings(int) {#constructor}

Задает настройки для метода сжатия LZMA2 в архиве 7z.

```csharp
public SevenZipLZMA2CompressionSettings(int dictionarySize = 16777216)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| dictionarySize | Int32 | Размер буфера истории должен быть между 4096 и 1073741824. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentOutOfRangeException | *dictionarySize* слишком велик или слишком мал. |

### Примечания

Чем больше словарь, тем обычно лучше степень сжатия, но словари большего размера, чем несжатые данные, являются пустой тратой оперативной памяти.

### Смотрите также

* class [SevenZipLZMA2CompressionSettings](../)
* пространство имен [Aspose.Zip.Saving](../../sevenziplzma2compressionsettings/)
* сборка [Aspose.Zip](../../../)

---

## SevenZipLZMA2CompressionSettings(int, int) {#constructor_1}

Задает настройки для метода сжатия LZMA2 в архиве 7z.

```csharp
public SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes = 32)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| dictionarySize | Int32 | Размер буфера истории должен быть между 4096 и 1073741824. |
| fastBytes | Int32 | Управляет количеством быстрых байтов, используемых компрессорами LZMA2. Большее количество быстрых байтов может обеспечить лучшую степень сжатия за счет скорости сжатия. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentOutOfRangeException | *dictionarySize* слишком большой или слишком маленький, или*fastBytes* слишком велик или слишком мал. |

### Примечания

Чем больше словарь, тем обычно лучше степень сжатия, но словари большего размера, чем несжатые данные, являются пустой тратой оперативной памяти.

### Смотрите также

* class [SevenZipLZMA2CompressionSettings](../)
* пространство имен [Aspose.Zip.Saving](../../sevenziplzma2compressionsettings/)
* сборка [Aspose.Zip](../../../)


