---
title: "XarEntry"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Представляет отдельную запись в архиве xar."
type: docs
weight: 140
url: /ru/java/com.aspose.zip/xarentry/
---

**Inheritance:**
java.lang.Object
```
public abstract class XarEntry
```

Представляет отдельную запись в архиве xar.
## Методы

| Метод | Описание |
| --- | --- |
| [getCreationTime()](#getCreationTime--) | Получает время создания файла или каталога. |
| [getFullPath()](#getFullPath--) | Получает полный путь к элементу внутри архива. |
| [getLastAccessTime()](#getLastAccessTime--) | Получает время последнего доступа к файлу или каталогу. |
| [getLastWriteTime()](#getLastWriteTime--) | Получает время модификации файла или каталога. |
| [getModificationTime()](#getModificationTime--) | Получает время модификации файла или каталога. |
| [getName()](#getName--) | Получает имя записи в архиве. |
| [getParent()](#getParent--) | Получает родительский каталог, к которому принадлежит запись. |
| [isDirectory()](#isDirectory--) | Получает значение, указывающее, является ли запись каталогом. |
| [toString()](#toString--) | Возвращает строковое представление экземпляра класса [XarEntry](../../com.aspose.zip/xarentry). |
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


Получает время создания файла или каталога.

**Returns:**
java.util.Date - время создания файла или каталога
### getFullPath() {#getFullPath--}
```
public final String getFullPath()
```


Получает полный путь к элементу внутри архива.

**Returns:**
java.lang.String - полный путь к элементу внутри архива
### getLastAccessTime() {#getLastAccessTime--}
```
public final Date getLastAccessTime()
```


Получает время последнего доступа к файлу или каталогу.

**Returns:**
java.util.Date - время последнего доступа к файлу или каталогу
### getLastWriteTime() {#getLastWriteTime--}
```
public final Date getLastWriteTime()
```


Получает время модификации файла или каталога.

**Returns:**
java.util.Date - время модификации файла или каталога
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Получает время модификации файла или каталога.

**Returns:**
java.util.Date - время модификации файла или каталога
### getName() {#getName--}
```
public final String getName()
```


Получает имя записи в архиве.

**Returns:**
java.lang.String - имя записи в архиве
### getParent() {#getParent--}
```
public final XarDirectoryEntry getParent()
```


Получает родительский каталог, к которому принадлежит запись.

**Returns:**
[XarDirectoryEntry](../../com.aspose.zip/xardirectoryentry) - the parent directory the entry belongs to
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


Возвращает строковое представление экземпляра класса [XarEntry](../../com.aspose.zip/xarentry).

**Returns:**
java.lang.String - строковое представление этого объекта
