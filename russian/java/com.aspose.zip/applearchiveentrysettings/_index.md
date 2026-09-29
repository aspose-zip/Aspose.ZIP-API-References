---
title: "AppleArchiveEntrySettings"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Настройки, используемые для создания записей внутри ."
type: docs
weight: 18
url: /ru/java/com.aspose.zip/applearchiveentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class AppleArchiveEntrySettings
```

Настройки, используемые для создания записей внутри [AppleArchive](../../com.aspose.zip/applearchive).
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [AppleArchiveEntrySettings(AppleCompressionSettings compressionSettings)](#AppleArchiveEntrySettings-com.aspose.zip.AppleCompressionSettings-) | Инициализирует новый экземпляр класса [AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings). |
## Методы

| Метод | Описание |
| --- | --- |
| [getCompressionSettings()](#getCompressionSettings--) | Получает настройки сжатия, применяемые к сформированной полезной нагрузке Apple Archive. |
| [getIncludeCrc32Checksum()](#getIncludeCrc32Checksum--) | Получает значение, указывающее, включены ли поля контрольной суммы CRC32 для сформированных файловых записей. |
| [setIncludeCrc32Checksum(boolean value)](#setIncludeCrc32Checksum-boolean-) | Устанавливает значение, указывающее, включены ли поля контрольной суммы CRC32 для сформированных файловых записей. |
### AppleArchiveEntrySettings(AppleCompressionSettings compressionSettings) {#AppleArchiveEntrySettings-com.aspose.zip.AppleCompressionSettings-}
```
public AppleArchiveEntrySettings(AppleCompressionSettings compressionSettings)
```


Инициализирует новый экземпляр класса [AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| compressionSettings | [AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings) | Настройки сжатия, применяемые к сформированной полезной нагрузке Apple Archive. |

### getCompressionSettings() {#getCompressionSettings--}
```
public final AppleCompressionSettings getCompressionSettings()
```


Получает настройки сжатия, применяемые к сформированной полезной нагрузке Apple Archive.

**Returns:**
[AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings) - compression settings applied to the composed Apple Archive payload.
### getIncludeCrc32Checksum() {#getIncludeCrc32Checksum--}
```
public final boolean getIncludeCrc32Checksum()
```


Получает значение, указывающее, включены ли поля контрольной суммы CRC32 для сформированных файловых записей.

**Returns:**
boolean — значение, указывающее, включены ли поля контрольной суммы CRC32 для сформированных файловых записей.
### setIncludeCrc32Checksum(boolean value) {#setIncludeCrc32Checksum-boolean-}
```
public final void setIncludeCrc32Checksum(boolean value)
```


Устанавливает значение, указывающее, включены ли поля контрольной суммы CRC32 для сформированных файловых записей.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean | значение, указывающее, включены ли поля контрольной суммы CRC32 для сформированных файловых записей. |

