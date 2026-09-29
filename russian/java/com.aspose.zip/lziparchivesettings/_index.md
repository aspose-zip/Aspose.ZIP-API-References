---
title: "LzipArchiveSettings"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Класс содержит настройки конкретного lzip‑архива."
type: docs
weight: 84
url: /ru/java/com.aspose.zip/lziparchivesettings/
---

**Inheritance:**
java.lang.Object
```
public class LzipArchiveSettings
```

Класс содержит настройки конкретного lzip‑архива.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [LzipArchiveSettings(int dictionarySize)](#LzipArchiveSettings-int-) | Инициализирует новый экземпляр [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) с определённым размером словаря. |
| [LzipArchiveSettings(int dictionarySize, int maxMemberSize)](#LzipArchiveSettings-int-int-) | Инициализирует новый экземпляр [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) с определённым размером словаря. |
## Методы

| Метод | Описание |
| --- | --- |
| [getCompressionThreads()](#getCompressionThreads--) | Получает количество потоков сжатия. |
| [getDictionarySize()](#getDictionarySize--) | Получает размер словаря, используемого при сжатии LZMA. |
| [getFastSpeed()](#getFastSpeed--) | Получает экземпляр класса [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) с размером словаря, равным 1 мегабайту, в фильтре LZMA. |
| [getFastestSpeed()](#getFastestSpeed--) | Получает экземпляр класса [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) с размером словаря, равным 65536 байт, в фильтре LZMA. |
| [getHighCompression()](#getHighCompression--) | Получает экземпляр класса [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) с размером словаря, равным 32 мегабайтам, в фильтре LZMA. |
| [getMaxMemberSize()](#getMaxMemberSize--) | Получает максимальный размер одного элемента в lzip-архиве в байтах. |
| [getMaximumCompression()](#getMaximumCompression--) | Получает экземпляр класса [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) с размером словаря, равным 64 мегабайтам, в фильтре LZMA. |
| [getNormal()](#getNormal--) | Получает экземпляр класса [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) с размером словаря, равным 16 мегабайтам, в фильтре LZMA. |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | Устанавливает количество потоков сжатия. |
### LzipArchiveSettings(int dictionarySize) {#LzipArchiveSettings-int-}
```
public LzipArchiveSettings(int dictionarySize)
```


Инициализирует новый экземпляр [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) с определённым размером словаря.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| dictionarySize | int | размер словаря для сжатия LZMA в байтах |

### LzipArchiveSettings(int dictionarySize, int maxMemberSize) {#LzipArchiveSettings-int-int-}
```
public LzipArchiveSettings(int dictionarySize, int maxMemberSize)
```


Инициализирует новый экземпляр [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) с определённым размером словаря.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| dictionarySize | int | размер словаря для сжатия LZMA в байтах |
| maxMemberSize | int | Максимальный размер одного элемента в lzip-архиве в байтах. Значение по умолчанию — 60 МБ. |

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


Получает размер словаря, используемого при сжатии LZMA.

**Returns:**
int - размер словаря, используемого при сжатии LZMA
### getFastSpeed() {#getFastSpeed--}
```
public static LzipArchiveSettings getFastSpeed()
```


Получает экземпляр класса [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) с размером словаря, равным 1 мегабайту, в фильтре LZMA.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 1 megabyte in LZMA filter
### getFastestSpeed() {#getFastestSpeed--}
```
public static LzipArchiveSettings getFastestSpeed()
```


Получает экземпляр класса [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) с размером словаря, равным 65536 байт, в фильтре LZMA.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 65536 bytes in LZMA filter
### getHighCompression() {#getHighCompression--}
```
public static LzipArchiveSettings getHighCompression()
```


Получает экземпляр класса [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) с размером словаря, равным 32 мегабайтам, в фильтре LZMA.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 32 megabytes in LZMA filter
### getMaxMemberSize() {#getMaxMemberSize--}
```
public final long getMaxMemberSize()
```


Получает максимальный размер одного элемента в lzip-архиве в байтах.

**Returns:**
long - максимальный размер одного элемента в lzip-архиве в байтах
### getMaximumCompression() {#getMaximumCompression--}
```
public static LzipArchiveSettings getMaximumCompression()
```


Получает экземпляр класса [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) с размером словаря, равным 64 мегабайтам, в фильтре LZMA.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 64 megabytes in LZMA filter
### getNormal() {#getNormal--}
```
public static LzipArchiveSettings getNormal()
```


Получает экземпляр класса [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) с размером словаря, равным 16 мегабайтам, в фильтре LZMA.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 16 megabytes in LZMA filter
### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


Устанавливает количество потоков сжатия. Если значение больше 1, будет использоваться многопоточное сжатие.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int | количество потоков сжатия |

