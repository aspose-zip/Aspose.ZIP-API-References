---
title: "CabEntrySettings"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Настройки, определяющие, как записывается запись CAB."
type: docs
weight: 47
url: /ru/java/com.aspose.zip/cabentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class CabEntrySettings
```

Настройки, определяющие, как записывается запись CAB.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [CabEntrySettings(CabCompressionSettings compressionSettings)](#CabEntrySettings-com.aspose.zip.CabCompressionSettings-) | Инициализирует настройки с определённым профилем сжатия. |
| [CabEntrySettings()](#CabEntrySettings--) | Инициализирует настройки с использованием сжатия MSZip по умолчанию. |
## Методы

| Метод | Описание |
| --- | --- |
| [getCompressionSettings()](#getCompressionSettings--) | Получает конфигурацию сжатия, применённую к элементу. |
### CabEntrySettings(CabCompressionSettings compressionSettings) {#CabEntrySettings-com.aspose.zip.CabCompressionSettings-}
```
public CabEntrySettings(CabCompressionSettings compressionSettings)
```


Инициализирует настройки с определённым профилем сжатия.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | compressionSettings | [CabCompressionSettings](../../com.aspose.zip/cabcompressionsettings) | Настройки сжатия для использования. |

Может быть одним из следующих: |

### CabEntrySettings() {#CabEntrySettings--}
```
public CabEntrySettings()
```


Инициализирует настройки с использованием сжатия MSZip по умолчанию.

### getCompressionSettings() {#getCompressionSettings--}
```
public final CabCompressionSettings getCompressionSettings()
```


Получает конфигурацию сжатия, применённую к элементу.

Может быть одним из следующих:

 *  

**Returns:**
[CabCompressionSettings](../../com.aspose.zip/cabcompressionsettings) - the compression configuration applied to the entry.
