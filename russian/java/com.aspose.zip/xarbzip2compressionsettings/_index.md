---
title: "XarBzip2CompressionSettings"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Настройки метода сжатия Bzip2."
type: docs
weight: 137
url: /ru/java/com.aspose.zip/xarbzip2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings)
```
public class XarBzip2CompressionSettings extends XarCompressionSettings
```

Настройки метода сжатия Bzip2.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [XarBzip2CompressionSettings(int blockSize)](#XarBzip2CompressionSettings-int-) | Инициализирует новый экземпляр класса [XarBzip2CompressionSettings](../../com.aspose.zip/xarbzip2compressionsettings). |
| [XarBzip2CompressionSettings()](#XarBzip2CompressionSettings--) | Инициализирует новый экземпляр класса [XarBzip2CompressionSettings](../../com.aspose.zip/xarbzip2compressionsettings) с размером блока по умолчанию, равным 9 сотням килобайт. |
## Методы

| Метод | Описание |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Размер блока в сотнях килобайт. |
### XarBzip2CompressionSettings(int blockSize) {#XarBzip2CompressionSettings-int-}
```
public XarBzip2CompressionSettings(int blockSize)
```


Инициализирует новый экземпляр класса [XarBzip2CompressionSettings](../../com.aspose.zip/xarbzip2compressionsettings).

```

``````

try (XarArchive archive = new XarArchive()) {
archive.createEntry("data.bin", "data.bin", false, new XarBzip2CompressionSettings(1));
archive.save("archive.xar");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| blockSize | int | block size in hundreds of kilobytes |

### XarBzip2CompressionSettings() {#XarBzip2CompressionSettings--}
```
public XarBzip2CompressionSettings()
```


Initializes a new instance of the [XarBzip2CompressionSettings](../../com.aspose.zip/xarbzip2compressionsettings) class with default block size, equals to 9 hundred of kilobytes.

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


Block size in hundreds of kilobytes.

**Returns:**
int - block size in hundreds of kilobytes
