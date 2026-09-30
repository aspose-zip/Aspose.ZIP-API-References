---
title: "Класс LzmaCompressionSettings"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Класс Aspose.Zip.Saving.LzmaCompressionSettings. Настройки сжатия LZMA в ZIP‑архиве"
type: docs
weight: 960
url: /ru/net/aspose.zip.saving/lzmacompressionsettings/
---
## LzmaCompressionSettings class

Настройки сжатия LZMA в архиве ZIP.

```csharp
public class LzmaCompressionSettings : CompressionSettings
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [LzmaCompressionSettings](lzmacompressionsettings/#constructor)() | Инициализирует новый экземпляр класса `LzmaCompressionSettings` с параметрами по умолчанию. |
| [LzmaCompressionSettings](lzmacompressionsettings/#constructor_1)(int) | Инициализирует новый экземпляр класса `LzmaCompressionSettings` с указанным размером словаря, количеством быстрых байтов по умолчанию, равным 32, и числом битов контекста литералов, равным 3. |
| [LzmaCompressionSettings](lzmacompressionsettings/#constructor_2)(int, int, int) | Инициализирует новый экземпляр класса `LzmaCompressionSettings` с указанным размером словаря, количеством быстрых байтов и количеством битов литерального контекста. |

## Свойства

| Имя | Описание |
| --- | --- |
| [DictionarySize](../../aspose.zip.saving/lzmacompressionsettings/dictionarysize/) { get; } | Размер словаря (буфера истории) указывает, сколько байтов недавно обработанных несжатых данных хранится в памяти. |
| [LiteralContextBits](../../aspose.zip.saving/lzmacompressionsettings/literalcontextbits/) { get; } | Возвращает количество битов литерального контекста. |
| [NumberOfFastBytes](../../aspose.zip.saving/lzmacompressionsettings/numberoffastbytes/) { get; } | Возвращает количество байтов, используемых для быстрого поиска совпадений в алгоритме LZMA. |

## Примечания

Алгоритм Лемпеля‑Зив‑Маркова (LZMA) — это алгоритм, используемый для выполнения без потерь сжатия данных. Этот алгоритм использует схему словарного сжатия, несколько похожую на алгоритм LZ77, и обладает высоким коэффициентом сжатия и переменным размером словаря сжатия.

Смотрите подробнее: [Алгоритм Лемпеля‑Зив‑Маркова](https://en.wikipedia.org/wiki/Lempel–Ziv–Markov_chain_algorithm)

### См. также

* class [CompressionSettings](../compressionsettings/)
* namespace [Aspose.Zip.Saving](../../aspose.zip.saving/)
* assembly [Aspose.Zip](../../)


