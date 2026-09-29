---
title: "SevenZipArchiveEntry"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Представляет отдельный файл внутри 7z‑архива."
type: docs
weight: 105
url: /ru/java/com.aspose.zip/sevenziparchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class SevenZipArchiveEntry implements IArchiveFileEntry
```

Представляет отдельный файл внутри 7z‑архива.

Преобразуйте экземпляр [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) в [SevenZipArchiveEntryEncrypted](../../com.aspose.zip/sevenziparchiveentryencrypted), чтобы определить, зашифрована ли запись.
## Методы

| Метод | Описание |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Извлекает запись в предоставленный поток. |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | Извлекает запись в предоставленный поток. |
| [extract(String path)](#extract-java.lang.String-) | Извлекает запись в файловую систему по указанному пути. |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | Извлекает запись в файловую систему по указанному пути. |
| [getCompressedSize()](#getCompressedSize--) | Получает размер сжатого файла. |
| [getCompressionProgressed()](#getCompressionProgressed--) | Получает событие, которое вызывается, когда часть необработанного потока сжата. |
| [getCompressionSettings()](#getCompressionSettings--) | Получает настройки для сжатия или распаковки. |
| [getLength()](#getLength--) | Получает длину. |
| [getModificationTime()](#getModificationTime--) | Получает дату и время последнего изменения. |
| [getName()](#getName--) | Получает имя записи в архиве. |
| [getUncompressedSize()](#getUncompressedSize--) | Получает размер оригинального файла. |
| [isDirectory()](#isDirectory--) | Получает значение, указывающее, является ли запись каталогом. |
| [open()](#open--) | Открывает запись для извлечения и предоставляет поток с содержимым записи. |
| [open(String password)](#open-java.lang.String-) | Открывает запись для извлечения и предоставляет поток с содержимым записи. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Устанавливает событие, которое вызывается, когда часть необработанного потока сжата. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Извлекает запись в предоставленный поток.

Извлечь запись из zip-архива с паролем.

```

``````

try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
archive.getEntries().get(0).extract(httpResponseStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream. Must be writable |

### extract(OutputStream destination, String password) {#extract-java.io.OutputStream-java.lang.String-}
```
public final void extract(OutputStream destination, String password)
```


Extracts the entry to the stream provided.

Extract an entry of zip archive with password.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
         archive.getEntries().get(0).extract(httpResponseStream);
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| назначение | java.io.OutputStream | поток назначения. Должен быть доступен для записи |
| password | java.lang.String | необязательный пароль для расшифровки |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Извлекает запись в файловую систему по указанному пути.

```

``````

try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
archive.getEntries().get(0).extract(\"data.bin\");
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

```

``````

     try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
         archive.getEntries().get(0).extract("data.bin");
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| path | java.lang.String | путь к целевому файлу. Если файл уже существует, он будет перезаписан. |
| password | java.lang.String | необязательный пароль для расшифровки |

**Returns:**
java.io.File — информация о извлечённом файле
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Получает размер сжатого файла.

**Returns:**
long - размер сжатого файла
### getCompressionProgressed() {#getCompressionProgressed--}
```
public final Event<ProgressEventArgs> getCompressionProgressed()
```


Получает событие, которое вызывается, когда часть необработанного потока сжата.

```

``````

archive.getEntries().get(0).setCompressionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
}
});
 
```

Event sender is an [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) instance.

Does not invoke in solid mode and in multithreaded mode for LZMA2 entries.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream compressed
### getCompressionSettings() {#getCompressionSettings--}
```
public final SevenZipCompressionSettings getCompressionSettings()
```


Gets settings for compression or decompression.

**Returns:**
[SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) - settings for compression or decompression
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets length.

**Returns:**
java.lang.Long - length
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Gets last modified date and time.

**Returns:**
java.util.Date - last modified date and time
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
long - the size of the original file
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Gets a value indicating whether the entry represents a directory.

**Returns:**
boolean - a value indicating whether the entry represents a directory
### open() {#open--}
```
public final InputStream open()
```


Opens the entry for extraction and provides a stream with entry content.

Usage:

```

``````

     SevenZipArchive archive = new SevenZipArchive("archive.7z");
     SevenZipArchiveEntry entry = archive.getEntries().get(0);
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

Прочитайте из потока, чтобы получить оригинальное содержимое файла. См. раздел примеров.

**Returns:**
java.io.InputStream - поток, представляющий содержимое записи.
### open(String password) {#open-java.lang.String-}
```
public final InputStream open(String password)
```


Открывает запись для извлечения и предоставляет поток с содержимым записи.

Использование:

```

``````

SevenZipArchive archive = new SevenZipArchive(\"archive.7z\");
SevenZipArchiveEntry entry = archive.getEntries().get(0);
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

Read from the stream to get the original content of the file. See examples section.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | java.lang.String | optional password for decryption |

**Returns:**
java.io.InputStream - the stream that represents the contents of the entry
### setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public final void setCompressionProgressed(Event<ProgressEventArgs> value)
```


Sets an event that is raised when a portion of raw stream compressed.

```

``````

    archive.getEntries().get(0).setCompressionProgressed(new Event<ProgressEventArgs>() {
        public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
            int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
        }
    });
 
```

Отправитель события является экземпляром [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry).

Не вызывается в solid‑режиме и в многопоточном режиме для записей LZMA2.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | событие, которое вызывается, когда часть необработанного потока сжата |

