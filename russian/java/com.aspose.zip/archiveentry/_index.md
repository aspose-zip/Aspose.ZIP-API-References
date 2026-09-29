---
title: "ArchiveEntry"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Представляет отдельный файл внутри архива."
type: docs
weight: 27
url: /ru/java/com.aspose.zip/archiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class ArchiveEntry implements IArchiveFileEntry
```

Представляет отдельный файл внутри архива.

Преобразуйте экземпляр [ArchiveEntry](../../com.aspose.zip/archiveentry) к [ArchiveEntryEncrypted](../../com.aspose.zip/archiveentryencrypted), чтобы определить, зашифрован ли элемент.
## Методы

| Метод | Описание |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Извлекает запись в предоставленный поток. |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | Извлекает запись в предоставленный поток. |
| [extract(String path)](#extract-java.lang.String-) | Извлекает запись в файловую систему по указанному пути. |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | Извлекает запись в файловую систему по указанному пути. |
| [getComment()](#getComment--) | Получает комментарий к элементу в архиве. |
| [getCompressedSize()](#getCompressedSize--) | Получает размер сжатого файла. |
| [getCompressionProgressed()](#getCompressionProgressed--) | Получает событие, которое вызывается, когда часть необработанного потока сжата. |
| [getCompressionSettings()](#getCompressionSettings--) | Получает настройки для сжатия или распаковки. |
| [getDataSource()](#getDataSource--) | Источник для элемента, если элемент был добавлен в архив, а не извлечён. |
| [getExtractionProgressed()](#getExtractionProgressed--) | Получает событие, которое вызывается, когда извлекается часть необработанного потока. |
| [getLength()](#getLength--) | Получает длину. |
| [getModificationTime()](#getModificationTime--) | Получает дату и время последнего изменения. |
| [getName()](#getName--) | Получает имя записи в архиве. |
| [getUncompressedSize()](#getUncompressedSize--) | Получает размер оригинального файла. |
| [isDirectory()](#isDirectory--) | Получает значение, указывающее, является ли запись каталогом. |
| [open()](#open--) | Открывает запись для извлечения и предоставляет поток с распакованным содержимым записи. |
| [open(String password)](#open-java.lang.String-) | Открывает запись для извлечения и предоставляет поток с распакованным содержимым записи. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Устанавливает событие, которое вызывается, когда часть необработанного потока сжата. |
| [setExtractionProgressed(Event&lt;ProgressCancelEventArgs&gt; value)](#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressCancelEventArgs--) | Устанавливает событие, которое вызывается, когда извлекается часть необработанного потока. |
| [setModificationTime(Date value)](#setModificationTime-java.util.Date-) | Устанавливает дату и время последнего изменения. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Извлекает запись в предоставленный поток.

Извлечь запись из zip-архива с паролем.

```

``````

try (FileInputStream zipFile = new FileInputStream("archive.zip")) {
try (Archive archive = new Archive(zipFile)) {
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

Extract an entry of zip archive with password.

```

``````

    try (FileInputStream zipFile = new FileInputStream("archive.zip")) {
        try (Archive archive = new Archive(zipFile)) {
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

Извлечь две записи из ZIP-архива, каждая со своим паролем

```

``````

try (FileInputStream zipFile = new FileInputStream("archive.zip")) {
try (Archive archive = new Archive(zipFile)) {
archive.getEntries().get(0).extract("first.bin", "first_pass");
archive.getEntries().get(1).extract("second.bin", "second_pass");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path to destination file. If the file already exists, it will be overwritten. |

**Returns:**
java.io.File - the file info of the extracted file
### extract(String path, String password) {#extract-java.lang.String-java.lang.String-}
```
public final File extract(String path, String password)
```


Extracts the entry to the filesystem by the path provided.

Extract two entries of ZIP archive, each with own password

```

``````

    try (FileInputStream zipFile = new FileInputStream("archive.zip")) {
        try (Archive archive = new Archive(zipFile)) {
            archive.getEntries().get(0).extract("first.bin", "first_pass");
            archive.getEntries().get(1).extract("second.bin", "second_pass");
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
### getComment() {#getComment--}
```
public final String getComment()
```


Получает комментарий к элементу в архиве.

**Returns:**
java.lang.String - комментарий записи в архиве
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

Event sender is an [ArchiveEntry](../../com.aspose.zip/archiveentry) instance.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream compressed
### getCompressionSettings() {#getCompressionSettings--}
```
public final CompressionSettings getCompressionSettings()
```


Gets settings for compression or decompression.

**Returns:**
[CompressionSettings](../../com.aspose.zip/compressionsettings) - settings for compression or decompression.
### getDataSource() {#getDataSource--}
```
public final InputStream getDataSource()
```


Source for the entry if the entry was added to the archive, not extracted.

Before assigned, the source is null. This source may be assigned within `Archive.save` method in some cases.

**Returns:**
java.io.InputStream - the source for the entry
### getExtractionProgressed() {#getExtractionProgressed--}
```
public final Event<ProgressCancelEventArgs> getExtractionProgressed()
```


Gets an event that is raised when a portion of raw stream extracted.

In this sample event handler is used for calculation the share of proceeded size in percents.

```

``````

    archive.getEntries().get(0).setExtractionProgressed(new Event<ProgressEventArgs>() {
        public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
            int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / ((ArchiveEntry) sender).getUncompressedSize());
        }
    });
 
```

В этом примере обработчик событий используется для отмены после извлечения первых сотни МБ записи.

```

``````

a.getEntries().get(0).setExtractionProgressed( (s, e) -> { if (e.getProceededBytes() > 100000000) e.setCancel(true); } );
 
```

Event sender is an [ArchiveEntry](../../com.aspose.zip/archiveentry) instance. It is possible to cancel extraction.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream extracted.
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


Gets name of the entry within the archive.

**Returns:**
java.lang.String - name of the entry within the archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets size of the original file.

**Returns:**
long - size of the original file
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

Читать из потока, чтобы получить оригинальное содержимое файла.

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
| password | java.lang.String | Optional password for decryption. |

**Returns:**
java.io.InputStream - The stream that represents the contents of the entry.
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

Отправитель события — это экземпляр [ArchiveEntry](../../com.aspose.zip/archiveentry).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | событие, которое вызывается, когда часть необработанного потока сжата |

### setExtractionProgressed(Event&lt;ProgressCancelEventArgs&gt; value) {#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressCancelEventArgs--}
```
public final void setExtractionProgressed(Event<ProgressCancelEventArgs> value)
```


Устанавливает событие, которое вызывается, когда извлекается часть необработанного потока.

В этом примере обработчик событий используется для расчёта доли обработанного размера в процентах.

```

``````

archive.getEntries().get(0).setExtractionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / ((ArchiveEntry) sender).getUncompressedSize());
}
});
 
```

In this sample event handler is used for cancellation after the first hundred of Mb of entry was extracted.

```

``````

 a.getEntries().get(0).setExtractionProgressed( (s, e) -> { if (e.getProceededBytes() > 100000000) e.setCancel(true); } );
 
```

Отправитель события — это экземпляр [ArchiveEntry](../../com.aspose.zip/archiveentry). Можно отменить извлечение.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | com.aspose.zip.Event&lt;com.aspose.zip.ProgressCancelEventArgs&gt; | событие, которое вызывается, когда часть необработанного потока извлечена. |

### setModificationTime(Date value) {#setModificationTime-java.util.Date-}
```
public final void setModificationTime(Date value)
```


Устанавливает дату и время последнего изменения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.util.Date | дата и время последнего изменения |

