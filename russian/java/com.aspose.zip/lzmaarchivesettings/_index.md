---
title: "LzmaArchiveSettings"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Настройки lzma‑архива."
type: docs
weight: 87
url: /ru/java/com.aspose.zip/lzmaarchivesettings/
---

**Inheritance:**
java.lang.Object
```
public class LzmaArchiveSettings
```

Настройки lzma‑архива.

Алгоритм Lempel\u2013Ziv\u2013Markov chain (LZMA) — это алгоритм, используемый для выполнения сжатия данных без потерь. Этот алгоритм использует схему словарного сжатия, отчасти похожую на алгоритм LZ77, и обладает высоким коэффициентом сжатия и переменным размером словаря сжатия.

Смотрите подробнее: [Lempel\u2013Ziv\u2013Markov chain algorithm][Lempel_u2013Ziv_u2013Markov chain algorithm]


[Lempel_u2013Ziv_u2013Markov chain algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [LzmaArchiveSettings()](#LzmaArchiveSettings--) | Инициализирует новый экземпляр класса [LzmaArchiveSettings](../../com.aspose.zip/lzmaarchivesettings) с размером словаря по умолчанию, равным 16 мегабайтам, количеством быстрых байтов, равным 32, и битами контекста литералов, равными 3. |
## Методы

| Метод | Описание |
| --- | --- |
| [getCompressionProgressed()](#getCompressionProgressed--) | Получает событие, которое вызывается, когда часть необработанного потока сжата. |
| [getDictionarySize()](#getDictionarySize--) | Размер словаря (буфера истории) указывает, сколько байтов недавно обработанных несжатых данных хранится в памяти. |
| [getLiteralContextBits()](#getLiteralContextBits--) | Возвращает количество битов контекста литералов. |
| [getNumberOfFastBytes()](#getNumberOfFastBytes--) | Возвращает количество байтов, используемых для быстрого поиска совпадений в алгоритме LZMA. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Устанавливает событие, которое вызывается, когда часть необработанного потока сжата. |
| [setDictionarySize(int value)](#setDictionarySize-int-) | Размер словаря (буфера истории) указывает, сколько байтов недавно обработанных несжатых данных хранится в памяти. |
| [setLiteralContextBits(int value)](#setLiteralContextBits-int-) | Устанавливает количество битов контекста литералов. |
| [setNumberOfFastBytes(int value)](#setNumberOfFastBytes-int-) | Устанавливает количество байтов, используемых для быстрого поиска совпадений в алгоритме LZMA. |
### LzmaArchiveSettings() {#LzmaArchiveSettings--}
```
public LzmaArchiveSettings()
```


Инициализирует новый экземпляр класса [LzmaArchiveSettings](../../com.aspose.zip/lzmaarchivesettings) с размером словаря по умолчанию, равным 16 мегабайтам, количеством быстрых байтов, равным 32, и битами контекста литералов, равными 3.

```

``````

LzmaArchiveSettings settings = new LzmaArchiveSettings();
settings.setDictionarySize(1048576);
try (LzmaArchive archive = new LzmaArchive(settings)) {
archive.setSource("data.bin");
archive.save(lzmaFile);
}
 
```



### getCompressionProgressed() {#getCompressionProgressed--}
```
public Event<ProgressEventArgs> getCompressionProgressed()
```


Gets an event that is raised when a portion of raw stream compressed.

```

``````

    lzmaArchiveSettings.setCompressionProgressed(new Event<ProgressEventArgs>() {
        public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
            int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
        }
    });
 
```



**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream compressed
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


Размер словаря (буфера истории) указывает, сколько байтов недавно обработанных несжатых данных хранится в памяти. Если не установлен, он будет выбран в соответствии с размером записи.

Чем больше словарь, тем обычно лучше коэффициент сжатия — но словари, превышающие размер несжатых данных, тратят ОЗУ зря. Размер словаря архива LZMA должен быть либо степенью двойки (2^n), либо в три раза больше степени двойки (3\*2^n).

**Returns:**
int — размер словаря (буфера истории).
### getLiteralContextBits() {#getLiteralContextBits--}
```
public final int getLiteralContextBits()
```


Возвращает количество битов контекста литералов.

Биты контекста литералов определяют, сколько из наиболее значимых битов предыдущего несжатого байта используется для предсказания битов следующего байта‑литерала. Должны быть в диапазоне от 0 до 8.

**Returns:**
int — количество битов контекста литералов.
### getNumberOfFastBytes() {#getNumberOfFastBytes--}
```
public final int getNumberOfFastBytes()
```


Возвращает количество байтов, используемых для быстрого поиска совпадений в алгоритме LZMA.

Большее значение позволяет компрессору искать более длинные совпадения, что может слегка улучшить коэффициент сжатия, но замедляет процесс сжатия.

**Returns:**
int — количество байтов, используемых для быстрого поиска совпадений в алгоритме LZMA.
### setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public void setCompressionProgressed(Event<ProgressEventArgs> value)
```


Устанавливает событие, которое вызывается, когда часть необработанного потока сжата.

```

``````

lzmaArchiveSettings.setCompressionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
}
});
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | an event that is raised when a portion of raw stream compressed |

### setDictionarySize(int value) {#setDictionarySize-int-}
```
public final void setDictionarySize(int value)
```


Dictionary (history buffer) size indicates how many bytes of the recently processed uncompressed data are kept in memory. If not set, will be chosen accordingly to entry size.

The bigger the dictionary, usually the better the compression ratio is - but dictionaries larger than the uncompressed data are a waste of RAM. The disctionary size of LZMA archive must be either a power of two (2^n) or three times a power of two (3\*2^n).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | Dictionary (history buffer) size. |

### setLiteralContextBits(int value) {#setLiteralContextBits-int-}
```
public final void setLiteralContextBits(int value)
```


Sets the number of literal context bits.

Literal Context Bits define how many of the most significant bits of the previous uncompressed byte are used to predict the bits of the next literal byte. Must be from 0 to 8.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the number of literal context bits. |

### setNumberOfFastBytes(int value) {#setNumberOfFastBytes-int-}
```
public final void setNumberOfFastBytes(int value)
```


Sets the number of bytes used for fast match searching in the LZMA algorithm.

A higher value allows the compressor to search longer matches, which can improve the compression ratio slightly but slows down compression.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the number of bytes used for fast match searching in the LZMA algorithm. |

