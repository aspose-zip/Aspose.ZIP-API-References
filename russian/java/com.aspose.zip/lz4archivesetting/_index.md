---
title: "Lz4ArchiveSetting"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Настройки формирования LZ4‑архива."
type: docs
weight: 81
url: /ru/java/com.aspose.zip/lz4archivesetting/
---

**Inheritance:**
java.lang.Object
```
public class Lz4ArchiveSetting
```

Настройки формирования LZ4‑архива.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [Lz4ArchiveSetting()](#Lz4ArchiveSetting--) | Инициализирует новый экземпляр [Lz4ArchiveSetting](../../com.aspose.zip/lz4archivesetting) с параметрами по умолчанию. |
## Методы

| Метод | Описание |
| --- | --- |
| [getIncludeBlockChecksum()](#getIncludeBlockChecksum--) | Возвращает значение, указывающее, следует ли включать сжатый xxh32 хеш в конце сжатого блока. |
| [getIncludeContentChecksum()](#getIncludeContentChecksum--) | Возвращает значение, указывающее, следует ли включать хеш содержимого xxh32 в конце архива LZ4. |
| [getIncludeContentSize()](#getIncludeContentSize--) | Возвращает значение, указывающее, следует ли включать размер содержимого в кадр. |
| [setIncludeBlockChecksum(boolean value)](#setIncludeBlockChecksum-boolean-) | Устанавливает значение, указывающее, следует ли включать сжатый xxh32 хеш в конце сжатого блока. |
| [setIncludeContentChecksum(boolean value)](#setIncludeContentChecksum-boolean-) | Устанавливает значение, указывающее, следует ли включать хеш содержимого xxh32 в конце архива LZ4. |
| [setIncludeContentSize(boolean value)](#setIncludeContentSize-boolean-) | Устанавливает значение, указывающее, следует ли включать размер содержимого в кадр. |
### Lz4ArchiveSetting() {#Lz4ArchiveSetting--}
```
public Lz4ArchiveSetting()
```


Инициализирует новый экземпляр [Lz4ArchiveSetting](../../com.aspose.zip/lz4archivesetting) с параметрами по умолчанию.

### getIncludeBlockChecksum() {#getIncludeBlockChecksum--}
```
public final boolean getIncludeBlockChecksum()
```


Возвращает значение, указывающее, следует ли включать сжатый xxh32 хеш в конце сжатого блока.

По умолчанию false.

**Returns:**
boolean — значение, указывающее, следует ли включать сжатый xxh32 хеш в конце сжатого блока.
### getIncludeContentChecksum() {#getIncludeContentChecksum--}
```
public final boolean getIncludeContentChecksum()
```


Возвращает значение, указывающее, следует ли включать хеш содержимого xxh32 в конце архива LZ4.

По умолчанию true.

**Returns:**
boolean - значение, указывающее, следует ли включать хеш xxh32 содержимого в конец архива LZ4.
### getIncludeContentSize() {#getIncludeContentSize--}
```
public final boolean getIncludeContentSize()
```


Возвращает значение, указывающее, следует ли включать размер содержимого в кадр.

По умолчанию false. Применяется, когда исходный поток поддерживает поиск.

**Returns:**
boolean - значение, указывающее, следует ли включать размер содержимого в кадр.
### setIncludeBlockChecksum(boolean value) {#setIncludeBlockChecksum-boolean-}
```
public final void setIncludeBlockChecksum(boolean value)
```


Устанавливает значение, указывающее, следует ли включать сжатый xxh32 хеш в конце сжатого блока.

По умолчанию false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean | значение, указывающее, следует ли включать сжатый хеш xxh32 в конец сжатого блока. |

### setIncludeContentChecksum(boolean value) {#setIncludeContentChecksum-boolean-}
```
public final void setIncludeContentChecksum(boolean value)
```


Устанавливает значение, указывающее, следует ли включать хеш содержимого xxh32 в конце архива LZ4.

По умолчанию true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean | значение, указывающее, следует ли включать хеш xxh32 содержимого в конец архива LZ4. |

### setIncludeContentSize(boolean value) {#setIncludeContentSize-boolean-}
```
public final void setIncludeContentSize(boolean value)
```


Устанавливает значение, указывающее, следует ли включать размер содержимого в кадр.

По умолчанию false. Применяется, когда исходный поток поддерживает поиск.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean | значение, указывающее, следует ли включать размер содержимого в кадр. |

