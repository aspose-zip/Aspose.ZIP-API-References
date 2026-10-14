---
title: "LhaArchiveEntry"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Представляет отдельный файл внутри архива Lha."
type: docs
weight: 76
url: /ru/java/com.aspose.zip/lhaarchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class LhaArchiveEntry implements IArchiveFileEntry
```

Представляет отдельный файл внутри архива Lha.
## Методы

| Метод | Описание |
| --- | --- |
| [extract(File file)](#extract-java.io.File-) | Извлекает запись архива Lha в файл. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Извлекает запись в предоставленный поток. |
| [extract(String path)](#extract-java.lang.String-) | Извлекает запись архива Lha в файловую систему по пути. |
| [getLastModified()](#getLastModified--) | Получает время последнего изменения записи. |
| [getLength()](#getLength--) | Получает длину записи в байтах. |
| [getModificationTime()](#getModificationTime--) | Получает время последнего изменения записи. |
| [getName()](#getName--) | Получает имя записи. |
| [getPath()](#getPath--) | Получает полный путь к записи. |
| [isDirectory()](#isDirectory--) | Получает значение, указывающее, является ли эта запись каталогом. |
### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Извлекает запись архива Lha в файл.

```

``````

try (FileInputStream lhaFile = new FileInputStream(\"archive.lha\")) {
try (LhaArchive archive = new LhaArchive(lhaFile)) {
archive.getEntries().get(0).extract(new File(\"extracted.bin\"));
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | File for storing decompressed data.

Does nothing for directory entry |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts the entry to the stream provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts Lha archive entry to a filesystem by path.

```

``````

     try (FileInputStream lhaFile = new FileInputStream("archive.lha")) {
         try (LhaArchive archive = new LhaArchive(lhaFile)) {
             archive.getEntries().get(0).extract("extracted.bin");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| path | java.lang.String | путь к файлу, в котором будут храниться распакованные данные |

**Returns:**
java.io.File - java.io.File instance containing extracted data
### getLastModified() {#getLastModified--}
```
public final Date getLastModified()
```


Получает время последнего изменения записи.

**Returns:**
java.util.Date — время последнего изменения записи
### getLength() {#getLength--}
```
public final Long getLength()
```


Получает длину записи в байтах.

**Returns:**
java.lang.Long — длина записи в байтах
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Получает время последнего изменения записи.

**Returns:**
java.util.Date — время последнего изменения записи
### getName() {#getName--}
```
public final String getName()
```


Получает имя записи.

Архивы только для сжатия, такие как gzip, bzip2, lzip, lzma, xz, z, имеют имя \"File.bin\", если в заголовках не найдено другое имя.

**Returns:**
java.lang.String - the name of the entry
### getPath() {#getPath--}
```
public final String getPath()
```


Получает полный путь к записи.

**Returns:**
java.lang.String — полный путь к записи
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Получает значение, указывающее, является ли эта запись каталогом.

**Returns:**
boolean — значение, указывающее, является ли эта запись каталогом.
