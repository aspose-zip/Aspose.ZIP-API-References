---
title: "IArchiveFileEntry"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Этот интерфейс представляет запись файла архива."
type: docs
weight: 162
url: /ru/java/com.aspose.zip/iarchivefileentry/
---
```
public interface IArchiveFileEntry
```

Этот интерфейс представляет запись файла архива.
## Методы

| Метод | Описание |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Извлекает запись в предоставленный поток. |
| [extract(String path)](#extract-java.lang.String-) | Извлекает запись в файловую систему по указанному пути. |
| [getLength()](#getLength--) | Получает длину записи в байтах. |
| [getName()](#getName--) | Получает имя записи. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public abstract void extract(OutputStream destination)
```


Извлекает запись в предоставленный поток.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| назначение | java.io.OutputStream | поток назначения. Должен быть доступен для записи |

### extract(String path) {#extract-java.lang.String-}
```
public abstract File extract(String path)
```


Извлекает запись в файловую систему по указанному пути.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| path | java.lang.String | путь к целевому файлу. Если файл уже существует, он будет перезаписан. |

**Returns:**
java.io.File - java.io.File instance containing extracted data
### getLength() {#getLength--}
```
public abstract Long getLength()
```


Получает длину записи в байтах.

**Returns:**
java.lang.Long — длина записи в байтах
### getName() {#getName--}
```
public abstract String getName()
```


Получает имя записи.

Архивы только для сжатия, такие как gzip, bzip2, lzip, lzma, xz, z, имеют имя \"File.bin\", если в заголовках не найдено другое имя.

**Returns:**
java.lang.String - the name of the entry
