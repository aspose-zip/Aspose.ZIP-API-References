---
title: "AppleLzmaCompressionSettings"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Настройки сжатия LZMA в файле Apple Archive .aar."
type: docs
weight: 23
url: /ru/java/com.aspose.zip/applelzmacompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings)
```
public class AppleLzmaCompressionSettings extends AppleCompressionSettings
```

Настройки сжатия LZMA в файле Apple Archive (.aar).
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [AppleLzmaCompressionSettings(int blockSize)](#AppleLzmaCompressionSettings-int-) | Инициализирует новый экземпляр класса [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings). |
| [AppleLzmaCompressionSettings(int blockSize, int dictionarySize)](#AppleLzmaCompressionSettings-int-int-) | Инициализирует новый экземпляр класса [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings). |
| [AppleLzmaCompressionSettings(int blockSize, int dictionarySize, int fastBytes)](#AppleLzmaCompressionSettings-int-int-int-) | Инициализирует новый экземпляр класса [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings). |
| [AppleLzmaCompressionSettings()](#AppleLzmaCompressionSettings--) | Инициализирует новый экземпляр класса [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) с параметрами по умолчанию. |
## Методы

| Метод | Описание |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Получает размер каждого блока данных до сжатия. |
| [getDictionarySize()](#getDictionarySize--) | Получает размер словаря, используемого для сжатия. |
| [getFastBytes()](#getFastBytes--) | Получает количество быстрых байтов, используемых для сжатия. |
### AppleLzmaCompressionSettings(int blockSize) {#AppleLzmaCompressionSettings-int-}
```
public AppleLzmaCompressionSettings(int blockSize)
```


Инициализирует новый экземпляр класса [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| blockSize | int | Размер каждого блока данных до сжатия. |

### AppleLzmaCompressionSettings(int blockSize, int dictionarySize) {#AppleLzmaCompressionSettings-int-int-}
```
public AppleLzmaCompressionSettings(int blockSize, int dictionarySize)
```


Инициализирует новый экземпляр класса [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| blockSize | int | Размер каждого блока данных до сжатия. |
| dictionarySize | int | Размер словаря, используемого для сжатия. |

### AppleLzmaCompressionSettings(int blockSize, int dictionarySize, int fastBytes) {#AppleLzmaCompressionSettings-int-int-int-}
```
public AppleLzmaCompressionSettings(int blockSize, int dictionarySize, int fastBytes)
```


Инициализирует новый экземпляр класса [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| blockSize | int | Размер каждого блока данных до сжатия. |
| dictionarySize | int | Размер словаря, используемого для сжатия. |
| fastBytes | int | Количество быстрых байтов, используемых для сжатия. |

### AppleLzmaCompressionSettings() {#AppleLzmaCompressionSettings--}
```
public AppleLzmaCompressionSettings()
```


Инициализирует новый экземпляр класса [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) с параметрами по умолчанию.

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


Получает размер каждого блока данных до сжатия.

Значение: значение по умолчанию равно 4 МиБ.

**Returns:**
int - размер каждого блока данных до сжатия.
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


Получает размер словаря, используемого для сжатия.

Значение: значение по умолчанию — 8 МиБ.

**Returns:**
int - размер словаря, используемого для сжатия.
### getFastBytes() {#getFastBytes--}
```
public final int getFastBytes()
```


Получает количество быстрых байтов, используемых для сжатия.

Значение: значение по умолчанию — 32.

**Returns:**
int - количество быстрых байтов, используемых для сжатия.
