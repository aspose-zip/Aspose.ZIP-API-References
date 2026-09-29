---
title: "SevenZipBZip2CompressionSettings"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Настройки метода сжатия BZip2 внутри 7z‑архива."
type: docs
weight: 109
url: /ru/java/com.aspose.zip/sevenzipbzip2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public class SevenZipBZip2CompressionSettings extends SevenZipCompressionSettings
```

Настройки метода сжатия BZip2 внутри 7z‑архива.

Bzip2 сжимает файлы, используя алгоритм текстового сжатия с блочным сортированием Бёрроуза-Уилера и кодирование Хаффмана.

Смотрите подробнее: [Bzip2][]


[Bzip2]: https://en.wikipedia.org/wiki/Bzip2
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [SevenZipBZip2CompressionSettings(int blockSize)](#SevenZipBZip2CompressionSettings-int-) | Инициализирует новый экземпляр класса [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings). |
| [SevenZipBZip2CompressionSettings()](#SevenZipBZip2CompressionSettings--) | Инициализирует новый экземпляр класса [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings) с размером блока по умолчанию, равным 9 сотням килобайт. |
## Методы

| Метод | Описание |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Размер блока в сотнях килобайт. |
| [getMethod()](#getMethod--) | Получает метод сжатия или распаковки. |
### SevenZipBZip2CompressionSettings(int blockSize) {#SevenZipBZip2CompressionSettings-int-}
```
public SevenZipBZip2CompressionSettings(int blockSize)
```


Инициализирует новый экземпляр класса [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| blockSize | int | размер блока в сотнях килобайт |

### SevenZipBZip2CompressionSettings() {#SevenZipBZip2CompressionSettings--}
```
public SevenZipBZip2CompressionSettings()
```


Инициализирует новый экземпляр класса [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings) с размером блока по умолчанию, равным 9 сотням килобайт.

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


Размер блока в сотнях килобайт.

**Returns:**
int — размер блока в сотнях килобайт
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


Получает метод сжатия или распаковки.

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method
