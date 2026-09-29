---
title: "RarArchiveEntry"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Представляет отдельный файл внутри архива."
type: docs
weight: 98
url: /ru/java/com.aspose.zip/rararchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class RarArchiveEntry implements IArchiveFileEntry
```

Представляет отдельный файл внутри архива.

Преобразуйте экземпляр [RarArchiveEntry](../../com.aspose.zip/rararchiveentry) к [RarArchiveEntryEncrypted](../../com.aspose.zip/rararchiveentryencrypted), чтобы определить, зашифрована ли запись.
## Методы

| Метод | Описание |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Извлекает запись в предоставленный поток. |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | Извлекает запись в предоставленный поток. |
| [extract(String path)](#extract-java.lang.String-) | Извлекает запись в файловую систему по указанному пути. |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | Извлекает запись в файловую систему по указанному пути. |
| [getCompressedSize()](#getCompressedSize--) | Получает размер сжатого файла. |
| [getCreationTime()](#getCreationTime--) | Получает дату и время создания. |
| [getExtractionProgressed()](#getExtractionProgressed--) | Получает событие, которое вызывается, когда извлекается часть необработанного потока. |
| [getLastAccessTime()](#getLastAccessTime--) | Получает дату и время последнего доступа. |
| [getLength()](#getLength--) | Получает длину. |
| [getModificationTime()](#getModificationTime--) | Получает дату и время последнего изменения. |
| [getName()](#getName--) | Получает имя записи в архиве. |
| [getUncompressedSize()](#getUncompressedSize--) | Получает размер оригинального файла. |
| [isDirectory()](#isDirectory--) | Получает значение, указывающее, является ли запись каталогом. |
| [open()](#open--) | Открывает запись для извлечения и предоставляет поток с распакованным содержимым записи. |
| [open(String password)](#open-java.lang.String-) | Открывает запись для извлечения и предоставляет поток с распакованным содержимым записи. |
| [setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Устанавливает событие, которое вызывается, когда извлекается часть необработанного потока. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Извлекает запись в предоставленный поток.


Извлекает запись из rar‑архива с паролем.

```

``````

try (FileInputStream rarFile = new FileInputStream("archive.rar")) {
try (RarArchive archive = new RarArchive(rarFile)) {
archive.getEntries().get(0).extract(outputStream, "p@s$");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | Destination stream. Must be writable. |

### extract(OutputStream destination, String password) {#extract-java.io.OutputStream-java.lang.String-}
```
public final void extract(OutputStream destination, String password)
```


Extracts the entry to the stream provided.


Extract an entry of rar archive with password.

```

``````

    try (FileInputStream rarFile = new FileInputStream("archive.rar")) {
        try (RarArchive archive = new RarArchive(rarFile)) {
            archive.getEntries().get(0).extract(outputStream, "p@s$");
        }
    } catch (IOException ex) {
    }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| назначение | java.io.OutputStream | Поток назначения. Должен быть доступен для записи. |
| password | java.lang.String | Необязательный пароль для расшифровки. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Извлекает запись в файловую систему по указанному пути.


Извлечь две записи из rar‑архива.

```

``````

try (FileInputStream rarFile = new FileInputStream("archive.rar")) {
try (RarArchive archive = new RarArchive(rarFile)) {
archive.getEntries().get(0).extract("first.bin", "pass");
archive.getEntries().get(1).extract("second.bin", "pass");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to destination file. If the file already exists, it will be overwritten |

**Returns:**
java.io.File - the file info of the extracted file
### extract(String path, String password) {#extract-java.lang.String-java.lang.String-}
```
public final File extract(String path, String password)
```


Extracts the entry to the filesystem by the path provided.


Extract two entries of rar archive.

```

``````

    try (FileInputStream rarFile = new FileInputStream("archive.rar")) {
        try (RarArchive archive = new RarArchive(rarFile)) {
            archive.getEntries().get(0).extract("first.bin", "pass");
            archive.getEntries().get(1).extract("second.bin", "pass");
        }
    } catch (IOException ex) {
    }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| path | java.lang.String | Путь к файлу назначения. Если файл уже существует, он будет перезаписан. |
| password | java.lang.String | Необязательный пароль для расшифровки. |

**Returns:**
java.io.File — информация о извлечённом файле
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Получает размер сжатого файла.

**Returns:**
long - размер сжатого файла
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


Получает дату и время создания.

**Returns:**
java.util.Date - дата и время создания.
### getExtractionProgressed() {#getExtractionProgressed--}
```
public final Event<ProgressEventArgs> getExtractionProgressed()
```


Получает событие, которое вызывается, когда извлекается часть необработанного потока.

```

``````

archive.getEntries().get(0).setExtractionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / ((RarArchiveEntry) sender).getUncompressedSize());
}
});
 
```

Event sender is an [RarArchiveEntry](../../com.aspose.zip/rararchiveentry) instance.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream extracted.
### getLastAccessTime() {#getLastAccessTime--}
```
public final Date getLastAccessTime()
```


Gets last access date and time.

**Returns:**
java.util.Date - last access date and time.
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets length.

**Returns:**
java.lang.Long - length.
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Gets last modified date and time.

**Returns:**
java.util.Date - last modified date and time.
### getName() {#getName--}
```
public final String getName()
```


Gets the name of the entry within the archive.

**Returns:**
java.lang.String - the name of the entry within the archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets the size of the original file.

**Returns:**
long - the size of the original file.
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Gets a value indicating whether the entry represents a directory.

**Returns:**
boolean - a value indicating whether the entry represents a directory.
### open() {#open--}
```
public final InputStream open()
```


Opens the entry for extraction and provides a stream with decompressed entry content.


Usage:

```

``````

    InputStream decompressed = entry.open();
    byte[] buffer = new byte[8192];
    int bytesRead;
    while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length)))
        fileStream.write(buffer, 0, bytesRead);
 
```

Прочитайте из потока, чтобы получить оригинальное содержимое файла. См. раздел примеров.

**Returns:**
java.io.InputStream - Поток, представляющий содержимое записи.
### open(String password) {#open-java.lang.String-}
```
public final InputStream open(String password)
```


Открывает запись для извлечения и предоставляет поток с распакованным содержимым записи.


Использование:

```

``````

InputStream decompressed = entry.open();
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length)))
fileStream.write(buffer, 0, bytesRead);
 
```

Read from the stream to get the original content of the file. See examples section.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | java.lang.String | Optional password for decryption. It can also be set within [RarArchiveLoadOptions.setDecryptionPassword(String)](../../com.aspose.zip/rararchiveloadoptions\#setDecryptionPassword-String-). |

**Returns:**
java.io.InputStream - The stream that represents the contents of the entry.
### setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public final void setExtractionProgressed(Event<ProgressEventArgs> value)
```


Sets an event that is raised when a portion of raw stream extracted.

```

``````

    archive.getEntries().get(0).setExtractionProgressed(new Event<ProgressEventArgs>() {
        public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
            int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / ((RarArchiveEntry) sender).getUncompressedSize());
        }
    });
 
```

Отправитель события является экземпляром [RarArchiveEntry](../../com.aspose.zip/rararchiveentry).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | событие, которое вызывается, когда часть необработанного потока извлечена. |

