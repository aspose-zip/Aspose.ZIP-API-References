---
title: "XarFileEntry"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Представляет запись файла в архиве xar."
type: docs
weight: 141
url: /ru/java/com.aspose.zip/xarfileentry/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.XarEntry](../../com.aspose.zip/xarentry)

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public final class XarFileEntry extends XarEntry implements IArchiveFileEntry
```

Представляет запись файла в архиве xar.
## Методы

| Метод | Описание |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Извлекает запись в предоставленный поток. |
| [extract(String path)](#extract-java.lang.String-) | Извлекает запись в файловую систему по указанному пути. |
| [getCompressionProgressed()](#getCompressionProgressed--) | Получает событие, которое вызывается, когда часть необработанного потока сжата. |
| [getLength()](#getLength--) | Получает длину записи в байтах. |
| [open()](#open--) | Открывает запись для извлечения и предоставляет поток с содержимым записи. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Устанавливает событие, которое вызывается, когда часть необработанного потока сжата. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Извлекает запись в предоставленный поток.

Извлечь запись из wim-архива.

```

``````

try (FileOutputStream output = new FileOutputStream(\"file\")){
try (XarArchive archive = new XarArchive(\"archive.xar\")) {
((XarFileEntry)archive.getEntries().get(0)).extract(output);
}
} catch (IOException ex) {
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

     try (XarArchive archive = new XarArchive("archive.xar")) {
         ((XarFileEntry)archive.getEntries().get(0)).extract("data.bin");
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| path | java.lang.String | путь к целевому файлу. Если файл уже существует, он будет перезаписан. |

**Returns:**
java.io.File — информация о извлечённом файле
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

Event sender is an [XarFileEntry](../../com.aspose.zip/xarfileentry) instance.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream compressed
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets the length of the entry in bytes.

**Returns:**
java.lang.Long - the length of the entry in bytes
### open() {#open--}
```
public final InputStream open()
```


Opens the entry for extraction and provides a stream with entry content.

Usage:

```

``````

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
### setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public final void setCompressionProgressed(Event<ProgressEventArgs> value)
```


Устанавливает событие, которое вызывается, когда часть необработанного потока сжата.

```

``````

archive.getEntries().get(0).setCompressionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
}
});
 
```

Event sender is an [XarFileEntry](../../com.aspose.zip/xarfileentry) instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | an event that is raised when a portion of raw stream compressed |

