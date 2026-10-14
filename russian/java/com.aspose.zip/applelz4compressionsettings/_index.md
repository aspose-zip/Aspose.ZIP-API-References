---
title: "AppleLz4CompressionSettings"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Настройки сжатия LZ4 в файле Apple Archive .aar."
type: docs
weight: 21
url: /ru/java/com.aspose.zip/applelz4compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings)
```
public class AppleLz4CompressionSettings extends AppleCompressionSettings
```

Настройки сжатия LZ4 в файле Apple Archive (.aar).
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [AppleLz4CompressionSettings(int blockSize)](#AppleLz4CompressionSettings-int-) | Инициализирует новый экземпляр класса [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings). |
| [AppleLz4CompressionSettings()](#AppleLz4CompressionSettings--) | Инициализирует новый экземпляр класса [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings) с параметрами по умолчанию. |
## Методы

| Метод | Описание |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Получает размер каждого сжатого блока `pbz4`/`bv41`. |
### AppleLz4CompressionSettings(int blockSize) {#AppleLz4CompressionSettings-int-}
```
public AppleLz4CompressionSettings(int blockSize)
```


Инициализирует новый экземпляр класса [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| blockSize | int | Размер каждого сжатого блока `pbz4`/`bv41`. |

### AppleLz4CompressionSettings() {#AppleLz4CompressionSettings--}
```
public AppleLz4CompressionSettings()
```


Инициализирует новый экземпляр класса [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings) с параметрами по умолчанию.

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


Получает размер каждого сжатого блока `pbz4`/`bv41`.

Значение: значение по умолчанию равно 4 МиБ.

**Returns:**
int - размер каждого сжатого блока `pbz4`/`bv41`.
