---
title: "Класс SevenZipLZMACompressionSettings"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Класс Aspose.Zip.Saving.SevenZipLZMACompressionSettings. Параметры метода сжатия LZMA в 7z‑архиве"
type: docs
weight: 1090
url: /ru/net/aspose.zip.saving/sevenziplzmacompressionsettings/
---
## SevenZipLZMACompressionSettings class

Настройки метода сжатия LZMA в архиве 7z.

```csharp
public class SevenZipLZMACompressionSettings : SevenZipCompressionSettings
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [SevenZipLZMACompressionSettings](sevenziplzmacompressionsettings/#constructor)() | Инициализирует новый экземпляр класса `SevenZipLZMACompressionSettings` с параметрами по умолчанию. |
| [SevenZipLZMACompressionSettings](sevenziplzmacompressionsettings/#constructor_1)(int) | Инициализирует новый экземпляр класса `SevenZipLZMACompressionSettings` с указанным размером словаря, количеством быстрых байтов, равным 32, и количеством битов контекста литералов, равным 3. |
| [SevenZipLZMACompressionSettings](sevenziplzmacompressionsettings/#constructor_2)(int, int, int) | Инициализирует новый экземпляр класса `SevenZipLZMACompressionSettings` с указанным размером словаря, количеством быстрых байтов и количеством битов контекста литералов. |

## Свойства

| Имя | Описание |
| --- | --- |
| [DictionarySize](../../aspose.zip.saving/sevenziplzmacompressionsettings/dictionarysize/) { get; set; } | Размер словаря (буфера истории) указывает, сколько байт недавно обработанных несжатых данных хранится в памяти. Если не задан, будет выбран в соответствии с размером записи. Должен быть от 4096 до 1073741824, либо равен нулю для автоматического определения на основе размера записи. |
| [LiteralContextBits](../../aspose.zip.saving/sevenziplzmacompressionsettings/literalcontextbits/) { get; } | Возвращает количество битов литерального контекста. |
| override [Method](../../aspose.zip.saving/sevenziplzmacompressionsettings/method/) { get; } | Получает метод сжатия или распаковки. |
| [NumberOfFastBytes](../../aspose.zip.saving/sevenziplzmacompressionsettings/numberoffastbytes/) { get; } | Возвращает количество байтов, используемых для быстрого поиска совпадений в алгоритме LZMA. |

## Примечания

Алгоритм Лемпеля‑Зив‑Маркова (LZMA) — это алгоритм, используемый для выполнения без потерь сжатия данных. Этот алгоритм использует схему словарного сжатия, несколько похожую на алгоритм LZ77, и обладает высоким коэффициентом сжатия и переменным размером словаря сжатия.

Смотрите подробнее: [Алгоритм Лемпеля‑Зив‑Маркова](https://en.wikipedia.org/wiki/Lempel–Ziv–Markov_chain_algorithm)

### См. также

* class [SevenZipCompressionSettings](../sevenzipcompressionsettings/)
* namespace [Aspose.Zip.Saving](../../aspose.zip.saving/)
* assembly [Aspose.Zip](../../)


