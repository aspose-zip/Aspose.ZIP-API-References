---
title: "LzxArchive"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Этот класс представляет файл архива LZX .lzx."
type: docs
weight: 89
url: /ru/java/com.aspose.zip/lzxarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class LzxArchive implements IArchive, AutoCloseable
```

Этот класс представляет файл архива LZX (.lzx).
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [LzxArchive(InputStream extractionSource)](#LzxArchive-java.io.InputStream-) | Инициализирует новый экземпляр класса [LzxArchive](../../com.aspose.zip/lzxarchive) и формирует список записей, которые могут быть извлечены из архива. |
| [LzxArchive(InputStream extractionSource, LzxLoadOptions loadOptions)](#LzxArchive-java.io.InputStream-com.aspose.zip.LzxLoadOptions-) | Инициализирует новый экземпляр класса [LzxArchive](../../com.aspose.zip/lzxarchive) и формирует список записей, которые могут быть извлечены из архива. |
| [LzxArchive(String path)](#LzxArchive-java.lang.String-) | Инициализирует новый экземпляр класса [LzxArchive](../../com.aspose.zip/lzxarchive) и формирует список записей, которые могут быть извлечены из архива. |
| [LzxArchive(String path, LzxLoadOptions loadOptions)](#LzxArchive-java.lang.String-com.aspose.zip.LzxLoadOptions-) | Инициализирует новый экземпляр класса [LzxArchive](../../com.aspose.zip/lzxarchive) и формирует список записей, которые могут быть извлечены из архива. |
## Методы

| Метод | Описание |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Извлекает все файлы и каталоги из архива в указанный каталог. |
| [getEntries()](#getEntries--) | Получает файловые записи типа [LzxArchiveEntry](../../com.aspose.zip/lzxarchiveentry), составляющие архив. |
| [getFileEntries()](#getFileEntries--) | Получает записи типа [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), составляющие архив. |
| [getFormat()](#getFormat--) | Получает формат архива. |
### LzxArchive(InputStream extractionSource) {#LzxArchive-java.io.InputStream-}
```
public LzxArchive(InputStream extractionSource)
```


Инициализирует новый экземпляр класса [LzxArchive](../../com.aspose.zip/lzxarchive) и формирует список записей, которые могут быть извлечены из архива.

Этот конструктор не распаковывает ни одну запись. См. метод [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\#extract-OutputStream-) для распаковки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| extractionSource | java.io.InputStream | Источник архива. |

### LzxArchive(InputStream extractionSource, LzxLoadOptions loadOptions) {#LzxArchive-java.io.InputStream-com.aspose.zip.LzxLoadOptions-}
```
public LzxArchive(InputStream extractionSource, LzxLoadOptions loadOptions)
```


Инициализирует новый экземпляр класса [LzxArchive](../../com.aspose.zip/lzxarchive) и формирует список записей, которые могут быть извлечены из архива.

Этот конструктор не распаковывает ни одну запись. См. метод [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\#extract-OutputStream-) для распаковки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| extractionSource | java.io.InputStream | Источник архива. |
| loadOptions | [LzxLoadOptions](../../com.aspose.zip/lzxloadoptions) | Параметры для загрузки существующего архива. |

### LzxArchive(String path) {#LzxArchive-java.lang.String-}
```
public LzxArchive(String path)
```


Инициализирует новый экземпляр класса [LzxArchive](../../com.aspose.zip/lzxarchive) и формирует список записей, которые могут быть извлечены из архива.

В следующем примере архив извлекается, затем первая запись распаковывается в `MemoryStream`.

```

``````

ByteArrayOutputStream extracted = new ByteArrayOutputStream();
try (LzxArchive archive = new LzxArchive(\"sample.lzx\")) {
archive.getEntries().get(0).extract(extracted);
}
 
```

This constructor does not decompress any entry. See [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The fully qualified or the relative path to the archive file. |

### LzxArchive(String path, LzxLoadOptions loadOptions) {#LzxArchive-java.lang.String-com.aspose.zip.LzxLoadOptions-}
```
public LzxArchive(String path, LzxLoadOptions loadOptions)
```


Initializes a new instance of the [LzxArchive](../../com.aspose.zip/lzxarchive) class and composes an entry list can be extracted from the archive.

The following example extracts an archive, then decompress first entry to a `MemoryStream`.

```

``````

     ByteArrayOutputStream extracted = new ByteArrayOutputStream();
     try (LzxArchive archive = new LzxArchive("sample.lzx")) {
         archive.getEntries().get(0).extract(extracted);
     }
 
```

Этот конструктор не распаковывает ни одну запись. См. метод [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\#extract-OutputStream-) для распаковки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| path | java.lang.String | Полный или относительный путь к файлу архива. |
| loadOptions | [LzxLoadOptions](../../com.aspose.zip/lzxloadoptions) | Параметры для загрузки существующего архива. |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Извлекает все файлы и каталоги из архива в указанный каталог.

```

``````

try (LzxArchive archive = new LzxArchive(\"archive.lzx\")) {
archive.extractToDirectory(\"C:/extracted\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | The path to the directory to place the extracted files in.

If the directory does not exist, it will be created. |

### getEntries() {#getEntries--}
```
public final List<LzxArchiveEntry> getEntries()
```


Gets file entries of [LzxArchiveEntry](../../com.aspose.zip/lzxarchiveentry) type constituting the archive.

**Returns:**
java.util.List&lt;com.aspose.zip.LzxArchiveEntry&gt; - file entries of [LzxArchiveEntry](../../com.aspose.zip/lzxarchiveentry) type constituting the archive.
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the archive
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Gets the archive format.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
