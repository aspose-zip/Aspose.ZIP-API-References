---
title: "Класс SevenZipLZMA2CompressionSettings"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Класс Aspose.Zip.Saving.SevenZipLZMA2CompressionSettings. Параметры метода сжатия LZMA2 в 7z‑архиве"
type: docs
weight: 1080
url: /ru/net/aspose.zip.saving/sevenziplzma2compressionsettings/
---
## SevenZipLZMA2CompressionSettings class

Настройки метода сжатия LZMA2 в архиве 7z.

```csharp
public class SevenZipLZMA2CompressionSettings : SevenZipCompressionSettings
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [SevenZipLZMA2CompressionSettings](sevenziplzma2compressionsettings/#constructor)(int) | Создаёт параметры метода сжатия LZMA2 в 7z‑архиве. |
| [SevenZipLZMA2CompressionSettings](sevenziplzma2compressionsettings/#constructor_1)(int, int) | Создаёт параметры метода сжатия LZMA2 в 7z‑архиве. |

## Свойства

| Имя | Описание |
| --- | --- |
| [CompressionThreads](../../aspose.zip.saving/sevenziplzma2compressionsettings/compressionthreads/) { get; set; } | Получает или задает количество потоков сжатия. Если значение больше 1, будет использоваться многопоточное сжатие. |
| [DictionarySize](../../aspose.zip.saving/sevenziplzma2compressionsettings/dictionarysize/) { get; } | Размер словаря (буфера истории) указывает, сколько байтов недавно обработанных несжатых данных хранится в памяти. |
| [FastBytes](../../aspose.zip.saving/sevenziplzma2compressionsettings/fastbytes/) { get; } | Возвращает контрольное число быстрых байтов, используемых компрессором LZMA2. |
| override [Method](../../aspose.zip.saving/sevenziplzma2compressionsettings/method/) { get; } | Получает метод сжатия или распаковки. |

## Примечания

LZMA2 поддерживает несколько запусков сжатых данных LZMA и несжатых данных.

Смотрите подробнее: [Алгоритм Лемпеля‑Зив‑Маркова](https://en.wikipedia.org/wiki/Lempel–Ziv–Markov_chain_algorithm)

### См. также

* class [SevenZipCompressionSettings](../sevenzipcompressionsettings/)
* namespace [Aspose.Zip.Saving](../../aspose.zip.saving/)
* assembly [Aspose.Zip](../../)


