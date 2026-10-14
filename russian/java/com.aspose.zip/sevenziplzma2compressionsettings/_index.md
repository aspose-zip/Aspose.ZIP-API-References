---
title: "SevenZipLZMA2CompressionSettings"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Настройки метода сжатия LZMA2 внутри 7z‑архива."
type: docs
weight: 114
url: /ru/java/com.aspose.zip/sevenziplzma2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public class SevenZipLZMA2CompressionSettings extends SevenZipCompressionSettings
```

Настройки метода сжатия LZMA2 внутри 7z‑архива.

LZMA2 поддерживает несколько запусков сжатых данных LZMA и несжатых данных.

Смотрите подробнее: [Lempel\\\\u2013Ziv\\\\u2013Markov\_chain\_algorithm][Lempel_u2013Ziv_u2013Markov_chain_algorithm]


[Lempel_u2013Ziv_u2013Markov_chain_algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [SevenZipLZMA2CompressionSettings()](#SevenZipLZMA2CompressionSettings--) | Создаёт экземпляр настроек для метода сжатия LZMA2 в архиве 7z. |
| [SevenZipLZMA2CompressionSettings(int dictionarySize)](#SevenZipLZMA2CompressionSettings-int-) | Создаёт экземпляр настроек для метода сжатия LZMA2 в архиве 7z. |
| [SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes)](#SevenZipLZMA2CompressionSettings-int-int-) | Создаёт экземпляр настроек для метода сжатия LZMA2 в архиве 7z. |
## Методы

| Метод | Описание |
| --- | --- |
| [getCompressionThreads()](#getCompressionThreads--) | Получает количество потоков сжатия. |
| [getDictionarySize()](#getDictionarySize--) | Размер словаря (буфера истории) указывает, сколько байтов недавно обработанных несжатых данных хранится в памяти. |
| [getFastBytes()](#getFastBytes--) | Получает контрольное число быстрых байтов, используемых компрессором LZMA2. |
| [getMethod()](#getMethod--) | Получает метод сжатия или распаковки. |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | Устанавливает количество потоков сжатия. |
### SevenZipLZMA2CompressionSettings() {#SevenZipLZMA2CompressionSettings--}
```
public SevenZipLZMA2CompressionSettings()
```


Создаёт экземпляр настроек для метода сжатия LZMA2 в архиве 7z.

### SevenZipLZMA2CompressionSettings(int dictionarySize) {#SevenZipLZMA2CompressionSettings-int-}
```
public SevenZipLZMA2CompressionSettings(int dictionarySize)
```


Создаёт экземпляр настроек для метода сжатия LZMA2 в архиве 7z.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | dictionarySize | int | Размер буфера истории, должен быть между 4096 и 1073741824. |

Чем больше словарь, тем обычно лучше коэффициент сжатия — но словари, превышающие размер несжатых данных, являются пустой тратой ОЗУ. |

### SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes) {#SevenZipLZMA2CompressionSettings-int-int-}
```
public SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes)
```


Создаёт экземпляр настроек для метода сжатия LZMA2 в архиве 7z.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | dictionarySize | int | Размер буфера истории, должен быть между 4096 и 1073741824. |

Чем больше словарь, тем обычно лучше коэффициент сжатия — но словари, превышающие размер несжатых данных, являются пустой тратой ОЗУ. |
| fastBytes | int | Контролирует количество быстрых байтов, используемых компрессорами LZMA2. Большее количество быстрых байтов может обеспечить лучший коэффициент сжатия за счёт скорости сжатия. |

### getCompressionThreads() {#getCompressionThreads--}
```
public final int getCompressionThreads()
```


Получает количество потоков сжатия. Если значение больше 1, будет использоваться многопоточное сжатие.

**Returns:**
int - количество потоков сжатия
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


Размер словаря (буфера истории) указывает, сколько байтов недавно обработанных несжатых данных хранится в памяти.

**Returns:**
int — размер словаря (буфера истории)
### getFastBytes() {#getFastBytes--}
```
public final int getFastBytes()
```


Получает контрольное число быстрых байтов, используемых компрессором LZMA2.

**Returns:**
int — контрольное число быстрых байтов, используемых компрессором LZMA2
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


Получает метод сжатия или распаковки.

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method.
### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


Устанавливает количество потоков сжатия. Если значение больше 1, будет использоваться многопоточное сжатие.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | int | количество потоков сжатия. |

Не устанавливайте это число больше количества ядер CPU. |

