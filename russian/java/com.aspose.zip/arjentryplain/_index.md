---
title: "ArjEntryPlain"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Представляет отдельный файл в архиве ARJ."
type: docs
weight: 38
url: /ru/java/com.aspose.zip/arjentryplain/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class ArjEntryPlain implements IArchiveFileEntry
```

Представляет отдельный файл в архиве ARJ.
## Методы

| Метод | Описание |
| --- | --- |
| [extract(File file)](#extract-java.io.File-) | Извлекает запись архива ARJ в файл. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Извлекает запись в предоставленный поток. |
| [extract(String path)](#extract-java.lang.String-) | Извлекает запись в файловую систему по указанному пути. |
| [getCompressedSize()](#getCompressedSize--) | Получает размер сжатого файла. |
| [getLength()](#getLength--) | Получает длину записи в байтах. |
| [getName()](#getName--) | Получает имя записи в архиве. |
| [getUncompressedSize()](#getUncompressedSize--) | Получает размер оригинального файла. |
### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Извлекает запись архива ARJ в файл.

```

``````

try (FileInputStream arjFile = new FileInputStream(\"sourceFileName\")) {
try (ArjArchive archive = new ArjArchive(arjFile)) {
archive.getEntries().get(0).extract(new File(\"extracted.bin\"));
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | java.io.File for storing decompressed data |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts the entry to the stream provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | Destination stream. Must be writable. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the entry to the filesystem by the path provided.

Extract two entries of rar archive.

```

``````

     try (FileInputStream arjFile = new FileInputStream("archive.arj")) {
         try (ArjArchive archive = new ArjArchive(arjFile)) {
             archive.getEntries().get(0).extract("first.bin");
             archive.getEntries().get(1).extract("second.bin");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| path | java.lang.String | путь к целевому файлу. Если файл уже существует, он будет перезаписан. |

**Returns:**
java.io.File - информация о файле составного файла
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Получает размер сжатого файла.

**Returns:**
long - размер сжатого файла
### getLength() {#getLength--}
```
public final Long getLength()
```


Получает длину записи в байтах.

**Returns:**
java.lang.Long — длина записи в байтах
### getName() {#getName--}
```
public final String getName()
```


Получает имя записи в архиве.

**Returns:**
java.lang.String - имя записи внутри архива
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Получает размер оригинального файла.

**Returns:**
long - размер оригинального файла
