---
title: "WimEntry"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Представляет отдельный файл или каталог в образе wim."
type: docs
weight: 132
url: /ru/java/com.aspose.zip/wimentry/
---

**Inheritance:**
java.lang.Object
```
public abstract class WimEntry
```

Представляет отдельный файл или каталог в образе wim.
## Методы

| Метод | Описание |
| --- | --- |
| [getAlternateDataStreams()](#getAlternateDataStreams--) | Получает имена альтернативных потоков данных для файла или каталога. |
| [getArchive()](#getArchive--) | Получает архив, к которому принадлежит запись. |
| [getChangeTime()](#getChangeTime--) | Получает время последнего изменения файла или каталога. |
| [getCreationTime()](#getCreationTime--) | Получает время создания файла или каталога. |
| [getFileAttributes()](#getFileAttributes--) | Получает атрибуты файла или каталога. |
| [getFullPath()](#getFullPath--) | Получает полный путь записи внутри образа. |
| [getHardLink()](#getHardLink--) | Получает идентификатор жесткой ссылки файла или каталога. |
| [getImage()](#getImage--) | Получает образ, к которому принадлежит запись. |
| [getLastAccessTime()](#getLastAccessTime--) | Получает время последнего доступа к файлу или каталогу. |
| [getLastWriteTime()](#getLastWriteTime--) | Получает время модификации файла или каталога. |
| [getModificationTime()](#getModificationTime--) | Получает время модификации файла или каталога. |
| [getName()](#getName--) | Получает имя записи внутри образа. |
| [getParent()](#getParent--) | Получает родительский каталог, к которому принадлежит запись. |
| [getShortName()](#getShortName--) | Получает короткое имя записи внутри образа. |
| [hasHardLinks()](#hasHardLinks--) | Определяет, известен ли файл или каталог под другими именами. |
| [isDirectory()](#isDirectory--) | Получает значение, указывающее, является ли запись каталогом. |
| [toString()](#toString--) | Возвращает строковое представление экземпляра класса [WimEntry](../../com.aspose.zip/wimentry). |
### getAlternateDataStreams() {#getAlternateDataStreams--}
```
public final String[] getAlternateDataStreams()
```


Получает имена альтернативных потоков данных для файла или каталога.

**Returns:**
java.lang.String[] - имена альтернативных потоков данных для файла или каталога
### getArchive() {#getArchive--}
```
public final WimArchive getArchive()
```


Получает архив, к которому принадлежит запись.

**Returns:**
[WimArchive](../../com.aspose.zip/wimarchive) - the archive the entry belongs to
### getChangeTime() {#getChangeTime--}
```
public final Date getChangeTime()
```


Получает время последнего изменения файла или каталога.

**Returns:**
java.util.Date - последнее время изменения файла или каталога
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


Получает время создания файла или каталога.

**Returns:**
java.util.Date - время создания файла или каталога
### getFileAttributes() {#getFileAttributes--}
```
public final int getFileAttributes()
```


Получает атрибуты файла или каталога.

**Returns:**
int - атрибуты файла или каталога
### getFullPath() {#getFullPath--}
```
public final String getFullPath()
```


Получает полный путь записи внутри образа.

**Returns:**
java.lang.String - полный путь к записи внутри образа
### getHardLink() {#getHardLink--}
```
public final long getHardLink()
```


Получает идентификатор жесткой ссылки файла или каталога.

**Returns:**
long - идентификатор жесткой ссылки файла или каталога
### getImage() {#getImage--}
```
public final WimImage getImage()
```


Получает образ, к которому принадлежит запись.

**Returns:**
[WimImage](../../com.aspose.zip/wimimage) - the image the entry belongs to
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


Получает имя записи внутри образа.

**Returns:**
java.lang.String - имя записи внутри образа
### getParent() {#getParent--}
```
public final WimDirectoryEntry getParent()
```


Получает родительский каталог, к которому принадлежит запись.

**Returns:**
[WimDirectoryEntry](../../com.aspose.zip/wimdirectoryentry) - the parent directory the entry belongs to
### getShortName() {#getShortName--}
```
public final String getShortName()
```


Получает короткое имя записи внутри образа.

**Returns:**
java.lang.String - короткое имя записи внутри образа
### hasHardLinks() {#hasHardLinks--}
```
public final boolean hasHardLinks()
```


Определяет, известен ли файл или каталог под другими именами.

**Returns:**
boolean - известен ли файл или каталог под другими именами
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


Возвращает строковое представление экземпляра класса [WimEntry](../../com.aspose.zip/wimentry).

**Returns:**
java.lang.String - строковое представление этого объекта
