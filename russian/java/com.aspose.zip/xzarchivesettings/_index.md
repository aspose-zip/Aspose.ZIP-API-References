---
title: "XzArchiveSettings"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Класс содержит набор настроек конкретного архива xz."
type: docs
weight: 147
url: /ru/java/com.aspose.zip/xzarchivesettings/
---

**Inheritance:**
java.lang.Object
```
public class XzArchiveSettings
```

Класс содержит набор настроек конкретного архива xz.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [XzArchiveSettings()](#XzArchiveSettings--) | Создаёт новый экземпляр класса [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings), используя одиночное сжатие LZMA2. |
| [XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType)](#XzArchiveSettings-com.aspose.zip.XzFilterSettings---long-com.aspose.zip.XzCheckType-) | Создаёт новый экземпляр класса [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) с пользовательскими параметрами. |
## Методы

| Метод | Описание |
| --- | --- |
| [getCompressionThreads()](#getCompressionThreads--) | Получает количество потоков сжатия. |
| [getFastSpeed()](#getFastSpeed--) | Возвращает экземпляр класса [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) с размером словаря 1 мегабайт в фильтре LZMA2, размером блока 4 мегабайта и контрольной суммой CRC32. |
| [getFastestSpeed()](#getFastestSpeed--) | Возвращает экземпляр класса [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) с размером словаря 65536 байт в фильтре LZMA2, размером блока 1 мегабайт и контрольной суммой CRC32. |
| [getHighCompression()](#getHighCompression--) | Возвращает экземпляр класса [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) с размером словаря 32 мегабайта в фильтре LZMA2, размером блока 128 мегабайт и контрольной суммой CRC32. |
| [getMaximumCompression()](#getMaximumCompression--) | Возвращает экземпляр класса [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) с размером словаря 64 мегабайта в фильтре LZMA2, размером блока 256 мегабайт и контрольной суммой CRC32. |
| [getNormal()](#getNormal--) | Возвращает экземпляр класса [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) с размером словаря 16 мегабайт в фильтре LZMA2, размером блока 64 мегабайта и контрольной суммой CRC32. |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | Устанавливает количество потоков сжатия. |
### XzArchiveSettings() {#XzArchiveSettings--}
```
public XzArchiveSettings()
```


Создаёт новый экземпляр класса [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings), используя одиночное сжатие LZMA2.

Словарь по умолчанию в фильтре LZMA2 имеет размер 16 мегабайт, размер блока по умолчанию — 64 мегабайта, тип контрольной суммы по умолчанию — CRC32.

### XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType) {#XzArchiveSettings-com.aspose.zip.XzFilterSettings---long-com.aspose.zip.XzCheckType-}
```
public XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType)
```


Создаёт новый экземпляр класса [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) с пользовательскими параметрами.

```

``````

try (FileOutputStream xzFile = new FileOutputStream("archive.xz")) {
XzLZMA2FilterSettings filter = new XzLZMA2FilterSettings(5242880);
XzArchiveSettings settings = new XzArchiveSettings(new XzFilterSettings[] {filter}, 10485760, XzCheckType.Crc32);
try (XzArchive archive = new XzArchive(settings)) {
archive.setSource("data.bin");
archive.save(xzFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filters | [XzFilterSettings\[\]](../../com.aspose.zip/xzfiltersettings) | filters (compressors) to be sequentially applied to create [XzArchive](../../com.aspose.zip/xzarchive). It can be either single [XzLZMA2FilterSettings](../../com.aspose.zip/xzlzma2filtersettings) or pair of [XzBcjX86FilterSettings](../../com.aspose.zip/xzbcjx86filtersettings) and [XzLZMA2FilterSettings](../../com.aspose.zip/xzlzma2filtersettings) |
| blockSize | long | size xz archive block |
| checkType | [XzCheckType](../../com.aspose.zip/xzchecktype) | type of checksum calculation for uncompressed data |

### getCompressionThreads() {#getCompressionThreads--}
```
public final int getCompressionThreads()
```


Gets compression thread count. If the value is greater than 1, multithreading compression will be used.

**Returns:**
int - compression thread count.
### getFastSpeed() {#getFastSpeed--}
```
public static XzArchiveSettings getFastSpeed()
```


Gets the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with dictionary size equals to 1 megabyte in LZMA2 filter, block size equals to 4 megabytes and CRC32 checksum.

**Returns:**
[XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) - the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with parameters for the fast speed
### getFastestSpeed() {#getFastestSpeed--}
```
public static XzArchiveSettings getFastestSpeed()
```


Gets the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with dictionary size equals to 65536 bytes in LZMA2 filter, block size equals to 1 megabyte and CRC32 checksum.

**Returns:**
[XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) - the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with parameters for the fastest speed
### getHighCompression() {#getHighCompression--}
```
public static XzArchiveSettings getHighCompression()
```


Gets the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with dictionary size equals to 32 megabytes in LZMA2 filter, block size equals to 128 megabytes and CRC32 checksum.

**Returns:**
[XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) - the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with parameters for the high compression
### getMaximumCompression() {#getMaximumCompression--}
```
public static XzArchiveSettings getMaximumCompression()
```


Gets the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with dictionary size equals to 64 megabytes in LZMA2 filter, block size equals to 256 megabytes and CRC32 checksum.

**Returns:**
[XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) - the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with parameters for the maximum compression
### getNormal() {#getNormal--}
```
public static XzArchiveSettings getNormal()
```


Gets the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with dictionary size equals to 16 megabytes in LZMA2 filter, block size equals to 64 megabytes and CRC32 checksum.

**Returns:**
[XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) - the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with normal parameters
### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


Sets compression thread count. If the value is greater than 1, multithreading compression will be used.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | compression thread count.

Do not set this number more than CPU cores |

