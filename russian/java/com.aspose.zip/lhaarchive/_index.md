---
title: "LhaArchive"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Этот класс представляет файл архива LHA .lzh."
type: docs
weight: 75
url: /ru/java/com.aspose.zip/lhaarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class LhaArchive implements IArchive, AutoCloseable
```

Этот класс представляет файл архива LHA (.lzh).

Поддерживаются только следующие методы сжатия:

| ------ | --------------------------------------------- |
| Method | Explanation                                   |
| lh0    | Несжатый                                      |
| lh4    | 8 КБ скользящий словарь и статический Хаффман |
| lh5    | 16 КБ скользящий словарь и статический Хаффман |
| lh6    | 64 КБ скользящий словарь и статический Хаффман |
| lh7    | 128 КБ скользящий словарь и статический Хаффман |
| lhx    | 1 МиБ скользящий словарь и статический Хаффман   |
| lhd    | Каталог                                      |
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [LhaArchive(InputStream sourceStream)](#LhaArchive-java.io.InputStream-) | Инициализирует новый экземпляр класса [LhaArchive](../../com.aspose.zip/lhaarchive) и формирует список записей, которые могут быть извлечены из архива. |
| [LhaArchive(InputStream sourceStream, LhaLoadOptions loadOptions)](#LhaArchive-java.io.InputStream-com.aspose.zip.LhaLoadOptions-) | Инициализирует новый экземпляр класса [LhaArchive](../../com.aspose.zip/lhaarchive) и формирует список записей, которые могут быть извлечены из архива. |
| [LhaArchive(String path)](#LhaArchive-java.lang.String-) | Инициализирует новый экземпляр класса [LhaArchive](../../com.aspose.zip/lhaarchive) и формирует список записей, которые могут быть извлечены из архива. |
| [LhaArchive(String path, LhaLoadOptions loadOptions)](#LhaArchive-java.lang.String-com.aspose.zip.LhaLoadOptions-) | Инициализирует новый экземпляр класса [LhaArchive](../../com.aspose.zip/lhaarchive) и формирует список записей, которые могут быть извлечены из архива. |
## Методы

| Метод | Описание |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Извлекает все файлы и каталоги из архива в указанный каталог. |
| [getEntries()](#getEntries--) | Получает файловые записи типа [LhaArchiveEntry](../../com.aspose.zip/lhaarchiveentry), составляющие архив. |
| [getFileEntries()](#getFileEntries--) | Получает записи типа [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), составляющие архив. |
| [getFormat()](#getFormat--) | Получает формат архива. |
### LhaArchive(InputStream sourceStream) {#LhaArchive-java.io.InputStream-}
```
public LhaArchive(InputStream sourceStream)
```


Инициализирует новый экземпляр класса [LhaArchive](../../com.aspose.zip/lhaarchive) и формирует список записей, которые могут быть извлечены из архива.

Этот конструктор не распаковывает ни одну запись. См. метод [LhaArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lhaarchiveentry\\#extract-OutputStream-) для распаковки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceStream | java.io.InputStream | источник архива |

### LhaArchive(InputStream sourceStream, LhaLoadOptions loadOptions) {#LhaArchive-java.io.InputStream-com.aspose.zip.LhaLoadOptions-}
```
public LhaArchive(InputStream sourceStream, LhaLoadOptions loadOptions)
```


Инициализирует новый экземпляр класса [LhaArchive](../../com.aspose.zip/lhaarchive) и формирует список записей, которые могут быть извлечены из архива.

Этот конструктор не распаковывает ни одну запись. См. метод [LhaArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lhaarchiveentry\\#extract-OutputStream-) для распаковки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceStream | java.io.InputStream | источник архива |
| loadOptions | [LhaLoadOptions](../../com.aspose.zip/lhaloadoptions) | Параметры для загрузки существующего архива. |

### LhaArchive(String path) {#LhaArchive-java.lang.String-}
```
public LhaArchive(String path)
```


Инициализирует новый экземпляр класса [LhaArchive](../../com.aspose.zip/lhaarchive) и формирует список записей, которые могут быть извлечены из архива.

В следующем примере архив извлекается, затем первая запись распаковывается в `MemoryStream`.

```

``````

ByteArrayOutputStream extracted = new ByteArrayOutputStream();
try (LhaArchive archive = new LhaArchive("sample.lzh")) {
archive.getEntries().get(0).extract(extracted);
}
 
```

This constructor does not decompress any entry. See [ArchiveEntry.extract(OutputStream)](../../com.aspose.zip/archiveentry\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the fully qualified or the relative path to the archive file |

### LhaArchive(String path, LhaLoadOptions loadOptions) {#LhaArchive-java.lang.String-com.aspose.zip.LhaLoadOptions-}
```
public LhaArchive(String path, LhaLoadOptions loadOptions)
```


Initializes a new instance of the [LhaArchive](../../com.aspose.zip/lhaarchive) class and composes an entry list can be extracted from the archive.

The following example extracts an archive, then decompress first entry to a `MemoryStream`.

```

``````

     ByteArrayOutputStream extracted = new ByteArrayOutputStream();
     try (LhaArchive archive = new LhaArchive("sample.lzh")) {
         archive.getEntries().get(0).extract(extracted);
     }
 
```

Этот конструктор не распаковывает ни одну запись. Смотрите метод [ArchiveEntry.extract(OutputStream)](../../com.aspose.zip/archiveentry\\#extract-OutputStream-) для распаковки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| path | java.lang.String | полный или относительный путь к файлу архива |
| loadOptions | [LhaLoadOptions](../../com.aspose.zip/lhaloadoptions) | Параметры для загрузки существующего архива. |

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

try (LhaArchive archive = new LhaArchive("archive.lzh")) {
archive.extractToDirectory(\"C:/extracted\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in.

If the directory does not exist, it will be created |

### getEntries() {#getEntries--}
```
public final List<LhaArchiveEntry> getEntries()
```


Gets file entries of [LhaArchiveEntry](../../com.aspose.zip/lhaarchiveentry) type constituting the archive.

**Returns:**
java.util.List&lt;com.aspose.zip.LhaArchiveEntry&gt; - file entries of [LhaArchiveEntry](../../com.aspose.zip/lhaarchiveentry) type constituting the archive
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
