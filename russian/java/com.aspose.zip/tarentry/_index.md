---
title: "TarEntry"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Представляет отдельный файл в архиве tar."
type: docs
weight: 126
url: /ru/java/com.aspose.zip/tarentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class TarEntry implements IArchiveFileEntry
```

Представляет отдельный файл в архиве tar.
## Методы

| Метод | Описание |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Извлекает запись в предоставленный поток. |
| [extract(String path)](#extract-java.lang.String-) | Извлекает запись в файловую систему по указанному пути. |
| [getLength()](#getLength--) | Получает длину записи в байтах. |
| [getModificationTime()](#getModificationTime--) | Получает время модификации файла или каталога. |
| [getName()](#getName--) | Получает имя записи в архиве. |
| [getUncompressedSize()](#getUncompressedSize--) | Получает размер исходного файла. |
| [isDirectory()](#isDirectory--) | Получает значение, указывающее, является ли запись каталогом. |
| [open()](#open--) | Открывает запись для извлечения и предоставляет поток с содержимым записи. |
| [setName(String value)](#setName-java.lang.String-) | Устанавливает имя записи в архиве. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Извлекает запись в предоставленный поток.

Извлечь запись из tar‑архива.

```

``````

try (TarArchive archive = new TarArchive("archive.tar")) {
archive.getEntries().get_Item(0).extract(httpResponseStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | Destination stream. Must be writable. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the entry to the filesystem by the path provided.

```

``````

     try (TarArchive archive = new TarArchive("archive.tar")) {
         archive.getEntries().get_Item(0).extract("data.bin");
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| path | java.lang.String | путь к целевому файлу. Если файл уже существует, он будет перезаписан. |

**Returns:**
java.io.File — информация о извлечённом файле
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


Получает время модификации файла или каталога.

**Returns:**
java.util.Date — время изменения файла или каталога.
### getName() {#getName--}
```
public final String getName()
```


Получает имя записи в архиве.

**Returns:**
java.lang.String - имя записи в архиве
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Получает размер исходного файла.

Имеет то же значение, что и `Length`([getLength](../../com.aspose.zip/tarentry\#getLength--))

**Returns:**
long — размер исходного файла.
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Получает значение, указывающее, является ли запись каталогом.

**Returns:**
boolean - a value indicating whether the entry represents a directory
### open() {#open--}
```
public final InputStream open()
```


Открывает запись для извлечения и предоставляет поток с содержимым записи.


Использование:

```

``````

InputStream decompressed = entry.open();
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
fileStream.write(buffer, 0, bytesRead);
}
 
```

Read from the stream to get the original content of the file. See examples section.

**Returns:**
java.io.InputStream - the stream that represents the contents of the entry
### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Sets the name of the entry within the archive.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the name of the entry within the archive |

