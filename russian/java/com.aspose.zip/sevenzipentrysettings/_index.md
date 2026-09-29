---
title: "SevenZipEntrySettings"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Настройки, используемые для сжатия или распаковки элементов 7z."
type: docs
weight: 113
url: /ru/java/com.aspose.zip/sevenzipentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class SevenZipEntrySettings
```

Настройки, используемые для сжатия или распаковки элементов 7z.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [SevenZipEntrySettings()](#SevenZipEntrySettings--) | Инициализирует новый экземпляр класса [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings). |
| [SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings)](#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-) | Инициализирует новый экземпляр класса [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings). |
| [SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings, SevenZipEncryptionSettings encryptionSettings)](#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-com.aspose.zip.SevenZipEncryptionSettings-) | Инициализирует новый экземпляр класса [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings). |
## Методы

| Метод | Описание |
| --- | --- |
| [getCompressHeader()](#getCompressHeader--) | Получает значение, указывающее, следует ли сжимать заголовок архива. |
| [getCompressionSettings()](#getCompressionSettings--) | Получает настройки для процедуры сжатия или распаковки. |
| [getEncryptionSettings()](#getEncryptionSettings--) | Получает настройки для шифрования или дешифрования. |
| [getSolid()](#getSolid--) | Получает значение, указывающее, следует ли объединять записи и рассматривать их как один блок данных. |
| [setCompressHeader(boolean value)](#setCompressHeader-boolean-) | Устанавливает значение, указывающее, следует ли сжимать заголовок архива. |
| [setSolid(boolean value)](#setSolid-boolean-) | Устанавливает значение, указывающее, следует ли объединять записи и рассматривать их как один блок данных. |
### SevenZipEntrySettings() {#SevenZipEntrySettings--}
```
public SevenZipEntrySettings()
```


Инициализирует новый экземпляр класса [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings).

### SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings) {#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-}
```
public SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings)
```


Инициализирует новый экземпляр класса [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | compressionSettings | [SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) | настройки для сжатия. Передайте null для использования настроек LZMA по умолчанию. |

Может быть одним из следующих:

 *  [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings)
 *  [SevenZipLZMA2CompressionSettings](../../com.aspose.zip/sevenziplzma2compressionsettings)
 *  [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings)
 *  [SevenZipPPMdCompressionSettings](../../com.aspose.zip/sevenzipppmdcompressionsettings)
 *  [SevenZipStoreCompressionSettings](../../com.aspose.zip/sevenzipstorecompressionsettings) |

### SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings, SevenZipEncryptionSettings encryptionSettings) {#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-com.aspose.zip.SevenZipEncryptionSettings-}
```
public SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings, SevenZipEncryptionSettings encryptionSettings)
```


Инициализирует новый экземпляр класса [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | compressionSettings | [SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) | настройки для сжатия. Передайте null для использования настроек LZMA по умолчанию. |

Может быть одним из следующих:

 *  [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings)
 *  [SevenZipLZMA2CompressionSettings](../../com.aspose.zip/sevenziplzma2compressionsettings)
 *  [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings)
 *  [SevenZipPPMdCompressionSettings](../../com.aspose.zip/sevenzipppmdcompressionsettings)
 *  [SevenZipStoreCompressionSettings](../../com.aspose.zip/sevenzipstorecompressionsettings) |
|  | encryptionSettings | [SevenZipEncryptionSettings](../../com.aspose.zip/sevenzipencryptionsettings) | настройки для шифрования. Передайте null, если нет необходимости шифровать или дешифровать. |

Может быть только один:

 *  [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) |

### getCompressHeader() {#getCompressHeader--}
```
public final boolean getCompressHeader()
```


Получает значение, указывающее, следует ли сжимать заголовок архива.

Эта настройка эквивалентна переключателю `-mhc=on` инструмента 7-Zip. В настоящее время она несовместима с шифрованием заголовка.

**Returns:**
boolean — значение, указывающее, следует ли сжимать заголовок архива
### getCompressionSettings() {#getCompressionSettings--}
```
public final SevenZipCompressionSettings getCompressionSettings()
```


Получает настройки для процедуры сжатия или распаковки.

**Returns:**
[SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) - settings for compression or decompression routine
### getEncryptionSettings() {#getEncryptionSettings--}
```
public final SevenZipEncryptionSettings getEncryptionSettings()
```


Получает настройки для шифрования или дешифрования. Настройки конкретной записи могут различаться.

Класс [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) — единственный вариант для архивов 7z.

**Returns:**
[SevenZipEncryptionSettings](../../com.aspose.zip/sevenzipencryptionsettings) - settings for encryption or decryption
### getSolid() {#getSolid--}
```
public final boolean getSolid()
```


Получает значение, указывающее, следует ли объединять записи и рассматривать их как один блок данных.

Следующий пример показывает, как сжать каталог в сплошной архив 7z с сжатием LZMA2 без шифрования.

```

``````

try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
SevenZipEntrySettings settings = new SevenZipEntrySettings(new SevenZipLZMACompressionSettings());
settings.setSolid(true);
try (SevenZipArchive archive = new SevenZipArchive(settings)) {
archive.createEntries("C:\\Documents");
archive.save(sevenZipFile);
}
} catch (IOException ex) {
}
 
```

Provide `SevenZipEntrySettings` for solid 7z archive on archive instantiation.

**Returns:**
boolean - value indicating whether to concatenate entries and treat them as a single data block.
### setCompressHeader(boolean value) {#setCompressHeader-boolean-}
```
public final void setCompressHeader(boolean value)
```


Sets value indicating whether to compress archive header.

This setting is equivalent `-mhc=on` switch of 7-Zip tool. Currently, it is incompatible with header encryption.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether to compress archive header |

### setSolid(boolean value) {#setSolid-boolean-}
```
public final void setSolid(boolean value)
```


Sets value indicating whether to concatenate entries and treat them as a single data block.

The following example shows how to compress a directory to solid 7z archive with LZMA2 compression without encryption.

```

``````

     try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
         SevenZipEntrySettings settings = new SevenZipEntrySettings(new SevenZipLZMACompressionSettings());
         settings.setSolid(true);
         try (SevenZipArchive archive = new SevenZipArchive(settings)) {
             archive.createEntries("C:\\Documents");
             archive.save(sevenZipFile);
         }
     } catch (IOException ex) {
     }
 
```

Предоставьте `SevenZipEntrySettings` для сплошного архива 7z при создании архива.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean | значение, указывающее, следует ли объединять записи и рассматривать их как один блок данных. |

