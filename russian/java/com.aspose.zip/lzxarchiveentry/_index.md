---
title: "LzxArchiveEntry"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Представляет отдельный файл внутри архива LZX."
type: docs
weight: 90
url: /ru/java/com.aspose.zip/lzxarchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class LzxArchiveEntry implements IArchiveFileEntry
```

Представляет отдельный файл внутри архива LZX.
## Методы

| Метод | Описание |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Извлекает запись в предоставленный поток. |
| [extract(String path)](#extract-java.lang.String-) | Извлекает запись архива Lzx в файловую систему по пути. |
| [getCommentary()](#getCommentary--) | Получает комментарий. |
| [getCompressedSize()](#getCompressedSize--) | Получает размер сжатого файла. |
| [getLength()](#getLength--) | Получает длину записи в байтах. |
| [getModificationTime()](#getModificationTime--) | Получает время последнего изменения записи. |
| [getName()](#getName--) | Получает имя записи. |
| [getUncompressedSize()](#getUncompressedSize--) | Получает размер оригинального файла. |
| [isDirectory()](#isDirectory--) | Получает значение, указывающее, является ли эта запись каталогом. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Извлекает запись в предоставленный поток.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| назначение | java.io.OutputStream | Поток назначения. Должен быть доступен для записи. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Извлекает запись архива Lzx в файловую систему по пути.

```

``````

try (FileInputStream lzxFile = new FileInputStream(\"archive.lzx\")) {
try (LzxArchive archive = new LzxArchive(lzxFile)) {
archive.getEntries().get(0).extract("extracted.bin");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | Path to file which will store decompressed data. |

**Returns:**
java.io.File - FileSystemInfoInstance containing extracted data.
### getCommentary() {#getCommentary--}
```
public final String getCommentary()
```


Gets the commentary.

**Returns:**
java.lang.String - the commentary.
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Gets size of the compressed file.

**Returns:**
long - size of the compressed file.
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets the length of the entry in bytes.

**Returns:**
java.lang.Long - the length of the entry in bytes
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Gets the last modified time of the entry.

**Returns:**
java.util.Date - the last modified time of the entry.
### getName() {#getName--}
```
public final String getName()
```


Gets the name of the entry.

Archives for compression only, such as gzip, bzip2, lzip, lzma, xz, z has name "File.bin" unless another name can be found in headers.

**Returns:**
java.lang.String - the name of the entry
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets size of the original file.

**Returns:**
long - size of the original file.
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Gets a value indicating whether this entry is a directory.

**Returns:**
boolean - a value indicating whether this entry is a directory.
