---
title: "AlzEntry"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Представляет файловый элемент в архиве ALZ вместе с его метаданными."
type: docs
weight: 13
url: /ru/java/com.aspose.zip/alzentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class AlzEntry implements IArchiveFileEntry
```

Представляет файловый элемент в архиве ALZ вместе с его метаданными.
## Методы

| Метод | Описание |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Извлекает запись в поток, доступный для записи. |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | Извлекает запись в поток, доступный для записи, используя необязательный пароль. |
| [extract(String path)](#extract-java.lang.String-) | Извлекает запись в указанный файл. |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | Извлекает запись в указанный файл, используя необязательный пароль. |
| [getCompressedSize()](#getCompressedSize--) | Возвращает сжатый размер данных записи в байтах. |
| [getLength()](#getLength--) | Возвращает несжатую длину этой записи. |
| [getName()](#getName--) | Возвращает имя записи, хранящееся в архиве. |
| [getUncompressedSize()](#getUncompressedSize--) | Возвращает несжатый размер данных записи в байтах. |
| [isDirectory()](#isDirectory--) | Возвращает, представляет ли эта запись каталог. |
| [open()](#open--) | Открывает запись и предоставляет поток, содержащий распакованные данные. |
| [open(String password)](#open-java.lang.String-) | Открывает запись и предоставляет поток, содержащий распакованные данные. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Извлекает запись в поток, доступный для записи.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| назначение | java.io.OutputStream | поток назначения |

### extract(OutputStream destination, String password) {#extract-java.io.OutputStream-java.lang.String-}
```
public final void extract(OutputStream destination, String password)
```


Извлекает запись в поток, доступный для записи, используя необязательный пароль.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| назначение | java.io.OutputStream | поток назначения |
| password | java.lang.String | необязательный пароль для этой записи |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Извлекает запись в указанный файл. Существующий файл будет перезаписан.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| path | java.lang.String | путь к файлу назначения |

**Returns:**
java.io.File - извлечённый файл
### extract(String path, String password) {#extract-java.lang.String-java.lang.String-}
```
public final File extract(String path, String password)
```


Извлекает запись в указанный файл, используя необязательный пароль.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| path | java.lang.String | путь к файлу назначения |
| password | java.lang.String | необязательный пароль для этой записи |

**Returns:**
java.io.File - извлечённый файл
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Возвращает сжатый размер данных записи в байтах.

**Returns:**
long - сжатый размер в байтах
### getLength() {#getLength--}
```
public final Long getLength()
```


Возвращает несжатую длину этой записи.

**Returns:**
java.lang.Long - несжатая длина в байтах
### getName() {#getName--}
```
public final String getName()
```


Возвращает имя записи, хранящееся в архиве.

**Returns:**
java.lang.String - имя записи
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Возвращает несжатый размер данных записи в байтах.

**Returns:**
long - несжатый размер в байтах
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Возвращает, представляет ли эта запись каталог.

**Returns:**
boolean - `true` для записи каталога
### open() {#open--}
```
public final InputStream open()
```


Открывает запись и предоставляет поток, содержащий распакованные данные.

**Returns:**
java.io.InputStream - поток, содержащий распакованные данные записи
### open(String password) {#open-java.lang.String-}
```
public final InputStream open(String password)
```


Открывает запись и предоставляет поток, содержащий распакованные данные.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| password | java.lang.String | необязательный пароль для этой записи |

**Returns:**
java.io.InputStream - поток, содержащий распакованные данные записи
