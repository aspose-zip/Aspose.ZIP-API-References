---
title: "CpioEntry"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Представляет отдельный файл в архиве cpio."
type: docs
weight: 58
url: /ru/java/com.aspose.zip/cpioentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public final class CpioEntry implements IArchiveFileEntry
```

Представляет отдельный файл в архиве cpio.
## Методы

| Метод | Описание |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Извлекает запись в предоставленный поток. |
| [extract(String path)](#extract-java.lang.String-) | Извлекает запись в файловую систему по указанному пути. |
| [getLastWriteTimeUtc()](#getLastWriteTimeUtc--) | Получает время последней записи. |
| [getLength()](#getLength--) | Получает длину записи в байтах. |
| [getName()](#getName--) | Получает имя записи в архиве. |
| [getParent()](#getParent--) | Получает архив, к которому принадлежит запись. |
| [isDirectory()](#isDirectory--) | Получает значение, указывающее, является ли запись каталогом. |
| [open()](#open--) | Открывает запись для извлечения и предоставляет поток с содержимым записи. |
| [toString()](#toString--) | Возвращает строковое представление экземпляра класса [CpioEntry](../../com.aspose.zip/cpioentry). |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Извлекает запись в предоставленный поток.

Извлечь запись из cpio-архива.

```

``````

try (CpioArchive archive = new CpioArchive("archive.cpio")) {
archive.getEntries().get(0).extract(httpResponseStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream. Must be writable |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the entry to the filesystem by the path provided.

```

``````

     try (CpioArchive archive = new CpioArchive("archive.cpio")) {
         archive.getEntries().get(0).extract("data.bin");
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| path | java.lang.String | путь к целевому файлу. Если файл уже существует, он будет перезаписан. |

**Returns:**
java.io.File — информация о извлечённом файле
### getLastWriteTimeUtc() {#getLastWriteTimeUtc--}
```
public final Date getLastWriteTimeUtc()
```


Получает время последней записи.

**Returns:**
java.util.Date - время последней записи
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
java.lang.String - имя записи в архиве
### getParent() {#getParent--}
```
public final CpioArchive getParent()
```


Получает архив, к которому принадлежит запись.

**Returns:**
[CpioArchive](../../com.aspose.zip/cpioarchive) - the archive the entry belongs to
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Получает значение, указывающее, является ли запись каталогом.

**Returns:**
boolean - значение, указывающее, представляет ли запись каталог.
### open() {#open--}
```
public final InputStream open()
```


Открывает запись для извлечения и предоставляет поток с содержимым записи.

Использование:

```

``````

CpioArchive archive = new CpioArchive("archive.cpio");
CpioEntry entry = archive.getEntries().get(0);
try (FileOutputStream fileStream = new FileOutputStream("data.bin")) {
try (InputStream decompressed = entry.open()) {
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
fileStream.write(buffer, 0, bytesRead);
}
}
} catch (IOException ex) {
}
 
```

Read from the stream to get the original content of a file. See examples section.

**Returns:**
java.io.InputStream - the stream that represents the contents of the entry
### toString() {#toString--}
```
public String toString()
```


Returns string representation of the instance of the [CpioEntry](../../com.aspose.zip/cpioentry) class.

**Returns:**
java.lang.String - string representation of this object.
