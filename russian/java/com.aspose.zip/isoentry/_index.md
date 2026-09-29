---
title: "IsoEntry"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Представляет файл или каталог записи внутри ISO-архива."
type: docs
weight: 72
url: /ru/java/com.aspose.zip/isoentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class IsoEntry implements IArchiveFileEntry
```

Представляет запись (файл или каталог) внутри ISO‑архива.
## Методы

| Метод | Описание |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Извлекает запись в предоставленный поток. |
| [extract(String path)](#extract-java.lang.String-) | Извлекает запись в файловую систему по указанному пути. |
| [getLength()](#getLength--) | Получает длину записи. |
| [getModificationTime()](#getModificationTime--) | Получает дату и время последнего изменения. |
| [getName()](#getName--) | Получает имя записи. |
| [isDirectory()](#isDirectory--) | Получает значение, указывающее, является ли запись каталогом. |
| [toString()](#toString--) | Возвращает строку, представляющую текущий элемент. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public void extract(OutputStream destination)
```


Извлекает запись в предоставленный поток.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| назначение | java.io.OutputStream | поток назначения |

### extract(String path) {#extract-java.lang.String-}
```
public File extract(String path)
```


Извлекает запись в файловую систему по указанному пути.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| path | java.lang.String | путь к файлу назначения. Если файл уже существует, он будет перезаписан. |

**Returns:**
java.io.File - java.io.File instance containing extracted data
### getLength() {#getLength--}
```
public Long getLength()
```


Получает длину записи.

**Returns:**
java.lang.Long - the length of the entry
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Получает дату и время последнего изменения.

**Returns:**
java.util.Date - last modified date and time
### getName() {#getName--}
```
public final String getName()
```


Получает имя записи.

**Returns:**
java.lang.String - the name of the entry
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Получает значение, указывающее, является ли запись каталогом.

**Returns:**
boolean - a value indicating whether the entry represents a directory
### toString() {#toString--}
```
public String toString()
```


Возвращает строку, представляющую текущий элемент.

**Returns:**
java.lang.String - the name of the entry
