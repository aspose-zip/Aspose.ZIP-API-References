---
title: "ArchiveEntrySettings"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Настройки, используемые для сжатия или распаковки элементов."
type: docs
weight: 30
url: /ru/java/com.aspose.zip/archiveentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class ArchiveEntrySettings
```

Настройки, используемые для сжатия или распаковки элементов.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [ArchiveEntrySettings()](#ArchiveEntrySettings--) | Создаёт новый экземпляр класса [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings). |
| [ArchiveEntrySettings(CompressionSettings compressionSettings)](#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-) | Создаёт новый экземпляр класса [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings). |
| [ArchiveEntrySettings(CompressionSettings compressionSettings, EncryptionSettings encryptionSettings)](#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-com.aspose.zip.EncryptionSettings-) | Создаёт новый экземпляр класса [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings). |
## Методы

| Метод | Описание |
| --- | --- |
| [getComment()](#getComment--) | Получает комментарий к записи в ZIP-архиве. |
| [getCompressionSettings()](#getCompressionSettings--) | Получает настройки для процедуры сжатия или распаковки. |
| [getEncryptionSettings()](#getEncryptionSettings--) | Получает настройки для шифрования или дешифрования. |
| [setComment(String value)](#setComment-java.lang.String-) | Комментарий к записи в ZIP-архиве. |
### ArchiveEntrySettings() {#ArchiveEntrySettings--}
```
public ArchiveEntrySettings()
```


Создаёт новый экземпляр класса [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings).

### ArchiveEntrySettings(CompressionSettings compressionSettings) {#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-}
```
public ArchiveEntrySettings(CompressionSettings compressionSettings)
```


Создаёт новый экземпляр класса [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | compressionSettings | [CompressionSettings](../../com.aspose.zip/compressionsettings) | Настройки сжатия. Передайте null для параметров дефляции по умолчанию. |

Может быть одним из следующих:

 *  [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings)
 *  [EnhancedDeflateCompressionSettings](../../com.aspose.zip/enhanceddeflatecompressionsettings)
 *  [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings) |

### ArchiveEntrySettings(CompressionSettings compressionSettings, EncryptionSettings encryptionSettings) {#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-com.aspose.zip.EncryptionSettings-}
```
public ArchiveEntrySettings(CompressionSettings compressionSettings, EncryptionSettings encryptionSettings)
```


Создаёт новый экземпляр класса [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | compressionSettings | [CompressionSettings](../../com.aspose.zip/compressionsettings) | Настройки сжатия. Передайте null для параметров дефляции по умолчанию. |

Может быть одним из следующих:

 *  [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings)
 *  [EnhancedDeflateCompressionSettings](../../com.aspose.zip/enhanceddeflatecompressionsettings)
 *  [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings) |
|  | encryptionSettings | [EncryptionSettings](../../com.aspose.zip/encryptionsettings) | Настройки шифрования. Передайте null, если нет необходимости шифровать или расшифровывать. |

Может быть одним из следующих:

 *  [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings)
 *  [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings) |

### getComment() {#getComment--}
```
public final String getComment()
```


Получает комментарий к записи в ZIP-архиве.

**Returns:**
java.lang.String — комментарий к записи в ZIP-архиве.
### getCompressionSettings() {#getCompressionSettings--}
```
public final CompressionSettings getCompressionSettings()
```


Получает настройки для процедуры сжатия или распаковки.

Может быть одним из следующих:

 *  [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings)
 *  [EnhancedDeflateCompressionSettings](../../com.aspose.zip/enhanceddeflatecompressionsettings)
 *  [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings)

**Returns:**
[CompressionSettings](../../com.aspose.zip/compressionsettings) - settings for compression or decompression routine.
### getEncryptionSettings() {#getEncryptionSettings--}
```
public final EncryptionSettings getEncryptionSettings()
```


Получает настройки для шифрования или дешифрования. Настройки конкретной записи могут различаться.

 *  [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings)
 *  [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings)

**Returns:**
[EncryptionSettings](../../com.aspose.zip/encryptionsettings) - settings for encryption or decryption. Settings of particular entry may vary.
### setComment(String value) {#setComment-java.lang.String-}
```
public final void setComment(String value)
```


Комментарий к записи в ZIP-архиве.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

