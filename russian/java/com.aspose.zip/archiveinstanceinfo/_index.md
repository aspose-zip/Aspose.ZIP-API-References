---
title: "ArchiveInstanceInfo"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Представляет информацию об экземпляре архива."
type: docs
weight: 34
url: /ru/java/com.aspose.zip/archiveinstanceinfo/
---

**Inheritance:**
java.lang.Object
```
public final class ArchiveInstanceInfo
```

Представляет информацию об экземпляре архива.
## Методы

| Метод | Описание |
| --- | --- |
| [areFileNamesEncrypted()](#areFileNamesEncrypted--) | Возвращает значение, указывающее, зашифрованы ли имена записей (файлов) архива. |
| [getArchiveFormatInfo(InputStream stream)](#getArchiveFormatInfo-java.io.InputStream-) | Возвращает информацию о формате архива. |
| [getArchiveFormatInfo(String fileName)](#getArchiveFormatInfo-java.lang.String-) | Возвращает информацию о формате архива. |
| [getArchiveInstanceInfo(InputStream stream)](#getArchiveInstanceInfo-java.io.InputStream-) | Возвращает информацию о экземпляре архива. |
| [getArchiveInstanceInfo(String fileName)](#getArchiveInstanceInfo-java.lang.String-) | Возвращает информацию о экземпляре архива. |
| [getFormatInfo()](#getFormatInfo--) | Возвращает информацию о формате архива. |
| [isContentEncrypted()](#isContentEncrypted--) | Получает значение, указывающее, зашифровано ли содержимое архива. |
### areFileNamesEncrypted() {#areFileNamesEncrypted--}
```
public final boolean areFileNamesEncrypted()
```


Возвращает значение, указывающее, зашифрованы ли имена записей (файлов) архива.

**Returns:**
boolean — значение, указывающее, зашифрованы ли имена записей (файлов) архива.
### getArchiveFormatInfo(InputStream stream) {#getArchiveFormatInfo-java.io.InputStream-}
```
public static ArchiveFormatInfo getArchiveFormatInfo(InputStream stream)
```


Возвращает информацию о формате архива.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | java.io.InputStream | Поток архивного файла. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format.
### getArchiveFormatInfo(String fileName) {#getArchiveFormatInfo-java.lang.String-}
```
public static ArchiveFormatInfo getArchiveFormatInfo(String fileName)
```


Возвращает информацию о формате архива.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | java.lang.String | Имя файла архива. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format.
### getArchiveInstanceInfo(InputStream stream) {#getArchiveInstanceInfo-java.io.InputStream-}
```
public static ArchiveInstanceInfo getArchiveInstanceInfo(InputStream stream)
```


Возвращает информацию о экземпляре архива.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | java.io.InputStream | Поток архивного файла. |

**Returns:**
[ArchiveInstanceInfo](../../com.aspose.zip/archiveinstanceinfo) - Information about archive instance or null if format was not detected.
### getArchiveInstanceInfo(String fileName) {#getArchiveInstanceInfo-java.lang.String-}
```
public static ArchiveInstanceInfo getArchiveInstanceInfo(String fileName)
```


Возвращает информацию о экземпляре архива.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | java.lang.String | Имя файла архива. |

**Returns:**
[ArchiveInstanceInfo](../../com.aspose.zip/archiveinstanceinfo) - Information about archive instance or null if format was not detected.
### getFormatInfo() {#getFormatInfo--}
```
public final ArchiveFormatInfo getFormatInfo()
```


Возвращает информацию о формате архива.

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - the archive format info.
### isContentEncrypted() {#isContentEncrypted--}
```
public final boolean isContentEncrypted()
```


Получает значение, указывающее, зашифровано ли содержимое архива.

**Returns:**
boolean — значение, указывающее, зашифровано ли содержимое архива.
