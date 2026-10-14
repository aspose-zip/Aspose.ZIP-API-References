---
title: "CabEntry"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Представляет отдельный файл в архиве CAB."
type: docs
weight: 46
url: /ru/java/com.aspose.zip/cabentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public final class CabEntry implements IArchiveFileEntry
```

Представляет отдельный файл в архиве CAB.
## Методы

| Метод | Описание |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Извлекает запись в предоставленный поток. |
| [extract(String path)](#extract-java.lang.String-) | Извлекает запись в файловую систему по указанному пути. |
| [getLength()](#getLength--) | Получает длину записи в байтах. |
| [getModificationTime()](#getModificationTime--) | Получает дату и время последнего изменения. |
| [getName()](#getName--) | Получает имя записи в архиве. |
| [open()](#open--) | Открывает запись для извлечения и предоставляет поток с содержимым записи. |
| [toString()](#toString--) | Возвращает строковое представление экземпляра класса [CabEntry](../../com.aspose.zip/cabentry). |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Извлекает запись в предоставленный поток.

Извлеките запись из архива CAB.

```

``````

try (CabArchive archive = new CabArchive("archive.cab")) {
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

     try (CabArchive archive = new CabArchive("archive.cab")) {
         archive.getEntries().get(0).extract("data.bin");
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| path | java.lang.String | путь к целевому файлу. Если файл уже существует, он будет перезаписан. |

**Returns:**
java.io.File - информация о файле составного файла
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


Получает дату и время последнего изменения.

**Returns:**
java.util.Date - дата и время последнего изменения.
### getName() {#getName--}
```
public final String getName()
```


Получает имя записи в архиве.

**Returns:**
java.lang.String - имя записи в архиве
### open() {#open--}
```
public final InputStream open()
```


Открывает запись для извлечения и предоставляет поток с содержимым записи.

Использование:

```

``````

CabArchive archive = new CabArchive(\"archive.cab\");
CabEntry entry = archive.getEntries().get(0);
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


Returns string representation of the instance of the [CabEntry](../../com.aspose.zip/cabentry) class.

**Returns:**
java.lang.String - string representation of this object
