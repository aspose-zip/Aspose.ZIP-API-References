---
title: "Класс LzmaArchiveSettings"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Класс Aspose.Zip.LZMA.LzmaArchiveSettings. Настройки для архива lzma"
type: docs
weight: 620
url: /ru/net/aspose.zip.lzma/lzmaarchivesettings/
---
## LzmaArchiveSettings class

Настройки архива lzma.

```csharp
public class LzmaArchiveSettings
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [LzmaArchiveSettings](lzmaarchivesettings/)() | Инициализирует новый экземпляр класса `LzmaArchiveSettings` с размером словаря по умолчанию, равным 16 мегабайтам, числом быстрых байтов, равным 32, и количеством битов контекста литералов, равным 3. |

## Свойства

| Имя | Описание |
| --- | --- |
| [DictionarySize](../../aspose.zip.lzma/lzmaarchivesettings/dictionarysize/) { get; set; } | Размер словаря (буфера истории) указывает, сколько байтов недавно обработанных несжатых данных хранится в памяти. Если не задан, будет выбран в соответствии с размером записи. |
| [LiteralContextBits](../../aspose.zip.lzma/lzmaarchivesettings/literalcontextbits/) { get; set; } | Получает или задает количество битов контекста литералов. |
| [NumberOfFastBytes](../../aspose.zip.lzma/lzmaarchivesettings/numberoffastbytes/) { get; set; } | Получает или задает количество байтов, используемых для быстрого поиска совпадений в алгоритме LZMA. |

## События

| Имя | Описание |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip.lzma/lzmaarchivesettings/compressionprogressed/) | Вызывается, когда часть необработанного потока сжата. |

## Примечания

Алгоритм Лемпеля‑Зив‑Маркова (LZMA) — это алгоритм, используемый для выполнения без потерь сжатия данных. Этот алгоритм использует схему словарного сжатия, несколько похожую на алгоритм LZ77, и обладает высоким коэффициентом сжатия и переменным размером словаря сжатия.

Смотрите подробнее: [Алгоритм Лемпеля‑Зив‑Маркова](https://en.wikipedia.org/wiki/Lempel–Ziv–Markov_chain_algorithm)

### См. также

* namespace [Aspose.Zip.LZMA](../../aspose.zip.lzma/)
* assembly [Aspose.Zip](../../)


