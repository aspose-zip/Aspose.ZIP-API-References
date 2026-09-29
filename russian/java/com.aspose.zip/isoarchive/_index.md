---
title: "IsoArchive"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Представляет ISO‑архив ISO 9660."
type: docs
weight: 71
url: /ru/java/com.aspose.zip/isoarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public final class IsoArchive implements IArchive, AutoCloseable
```

Представляет ISO‑архив (ISO 9660).
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [IsoArchive()](#IsoArchive--) | Инициализирует новый экземпляр класса [IsoArchive](../../com.aspose.zip/isoarchive) и создает пустой ISO‑архив для добавления новых файлов и каталогов. |
| [IsoArchive(InputStream sourceStream)](#IsoArchive-java.io.InputStream-) | Инициализирует новый экземпляр класса [IsoArchive](../../com.aspose.zip/isoarchive) и формирует список записей, которые можно извлечь из архива. |
| [IsoArchive(InputStream sourceStream, IsoLoadOptions loadOptions)](#IsoArchive-java.io.InputStream-com.aspose.zip.IsoLoadOptions-) | Инициализирует новый экземпляр класса [IsoArchive](../../com.aspose.zip/isoarchive) и формирует список записей, которые можно извлечь из архива. |
| [IsoArchive(String path)](#IsoArchive-java.lang.String-) | Инициализирует новый экземпляр класса [IsoArchive](../../com.aspose.zip/isoarchive) и формирует список записей, которые можно извлечь из архива. |
| [IsoArchive(String path, IsoLoadOptions loadOptions)](#IsoArchive-java.lang.String-com.aspose.zip.IsoLoadOptions-) | Инициализирует новый экземпляр класса [IsoArchive](../../com.aspose.zip/isoarchive) и формирует список записей, которые можно извлечь из архива. |
## Методы

| Метод | Описание |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createDirectory(String name)](#createDirectory-java.lang.String-) | Добавляет каталог в ISO‑образ. |
| [createEntry(String name)](#createEntry-java.lang.String-) | Добавляет файл в ISO‑образ. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | Добавляет файл в ISO‑образ. |
| [createEntry(String name, String filePath)](#createEntry-java.lang.String-java.lang.String-) | Добавляет файл в ISO‑образ. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Извлекает все записи в указанный каталог. |
| [getEntries()](#getEntries--) | Получает записи типа [IsoEntry](../../com.aspose.zip/isoentry), составляющие архив. |
| [getFileEntries()](#getFileEntries--) | Получает записи типа [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), составляющие архив. |
| [getFormat()](#getFormat--) | Получает формат архива. |
| [save(OutputStream stream)](#save-java.io.OutputStream-) | Сохраняет ISO‑образ в указанный поток. |
| [save(OutputStream stream, IsoSaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.IsoSaveOptions-) | Сохраняет ISO‑образ в указанный поток. |
| [save(String path)](#save-java.lang.String-) | Сохраняет ISO‑образ по указанному пути. |
| [save(String path, IsoSaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.IsoSaveOptions-) | Сохраняет ISO‑образ по указанному пути. |
### IsoArchive() {#IsoArchive--}
```
public IsoArchive()
```


Инициализирует новый экземпляр класса [IsoArchive](../../com.aspose.zip/isoarchive) и создает пустой ISO‑архив для добавления новых файлов и каталогов.

В следующем примере показано, как создать новый пустой ISO‑архив и добавить в него файлы:

```

``````

// Создать новый пустой ISO‑архив
try (IsoArchive isoArchive = new IsoArchive()) {
// Добавить файлы в ISO‑архив
isoArchive.createEntry("example_file.txt", "path_to_file.txt");
// Сохранить ISO‑архив в файл
isoArchive.save("new_archive.iso");
}
 
```



### IsoArchive(InputStream sourceStream) {#IsoArchive-java.io.InputStream-}
```
public IsoArchive(InputStream sourceStream)
```


Initializes a new instance of the [IsoArchive](../../com.aspose.zip/isoarchive) class and composes an entry list that can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (IsoArchive archive = new IsoArchive(new FileInputStream("archive.iso"))) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

Этот конструктор не распаковывает ни одну запись.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceStream | java.io.InputStream | источник архива |

### IsoArchive(InputStream sourceStream, IsoLoadOptions loadOptions) {#IsoArchive-java.io.InputStream-com.aspose.zip.IsoLoadOptions-}
```
public IsoArchive(InputStream sourceStream, IsoLoadOptions loadOptions)
```


Инициализирует новый экземпляр класса [IsoArchive](../../com.aspose.zip/isoarchive) и формирует список записей, которые можно извлечь из архива.

В следующем примере показано, как извлечь все записи в каталог.

```

``````

try (IsoArchive archive = new IsoArchive(new FileInputStream("archive.iso"))) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |
| loadOptions | [IsoLoadOptions](../../com.aspose.zip/isoloadoptions) | the options to load archive with |

### IsoArchive(String path) {#IsoArchive-java.lang.String-}
```
public IsoArchive(String path)
```


Initializes a new instance of the [IsoArchive](../../com.aspose.zip/isoarchive) class and composes an entry list that can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (IsoArchive archive = new IsoArchive("archive.iso")) {
         archive.extractToDirectory("C:\\extracted");
     }
 
```

Этот конструктор не распаковывает ни одну запись.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| path | java.lang.String | путь к файлу архива |

### IsoArchive(String path, IsoLoadOptions loadOptions) {#IsoArchive-java.lang.String-com.aspose.zip.IsoLoadOptions-}
```
public IsoArchive(String path, IsoLoadOptions loadOptions)
```


Инициализирует новый экземпляр класса [IsoArchive](../../com.aspose.zip/isoarchive) и формирует список записей, которые можно извлечь из архива.

В следующем примере показано, как извлечь все записи в каталог.

```

``````

try (IsoArchive archive = new IsoArchive("archive.iso")) {
archive.extractToDirectory("C:\\extracted");
}
 
```

This constructor does not unpack any entry.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |
| loadOptions | [IsoLoadOptions](../../com.aspose.zip/isoloadoptions) | the options to load archive with |

### close() {#close--}
```
public void close()
```




### createDirectory(String name) {#createDirectory-java.lang.String-}
```
public final IsoEntry createDirectory(String name)
```


Adds a directory to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the directory in the ISO |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### createEntry(String name) {#createEntry-java.lang.String-}
```
public final IsoEntry createEntry(String name)
```


Adds a file to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the file in the ISO |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final IsoEntry createEntry(String name, InputStream source)
```


Adds a file to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the file in the ISO |
| source | java.io.InputStream | the stream containing the file data |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### createEntry(String name, String filePath) {#createEntry-java.lang.String-java.lang.String-}
```
public final IsoEntry createEntry(String name, String filePath)
```


Adds a file to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the file in the ISO |
| filePath | java.lang.String | the path of the file |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all entries to the specified directory.

The following example shows how to extract all entries to a directory:

```

``````

     try (IsoArchive archive = new IsoArchive(new FileInputStream("archive.iso"))) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| destinationDirectory | java.lang.String | директория, в которую извлекать записи |

### getEntries() {#getEntries--}
```
public final List<IsoEntry> getEntries()
```


Получает записи типа [IsoEntry](../../com.aspose.zip/isoentry), составляющие архив.

**Returns:**
java.util.List&lt;com.aspose.zip.IsoEntry&gt; - элементы типа [IsoEntry](../../com.aspose.zip/isoentry), составляющие iso-архив
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Получает записи типа [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), составляющие архив.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - элементы типа [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), составляющие iso-архив
### getFormat() {#getFormat--}
```
public ArchiveFormat getFormat()
```


Получает формат архива.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream stream)
```


Сохраняет ISO‑образ в указанный поток.

Следующий пример показывает, как сохранить ISO-архив в поток памяти:

```

``````

ByteArrayOutputStream memoryStream = new ByteArrayOutputStream();
// Создать новый пустой ISO‑архив
try (IsoArchive isoArchive = new IsoArchive()) {
// Добавить файлы в ISO‑архив
isoArchive.createEntry("example_file.txt", "path_to_file.txt");
// Сохранить ISO-архив в поток памяти
isoArchive.save(memoryStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | the stream where the ISO image will be saved |

### save(OutputStream stream, IsoSaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.IsoSaveOptions-}
```
public final void save(OutputStream stream, IsoSaveOptions saveOptions)
```


Saves the ISO image to the specified stream.

The following example shows how to save an ISO archive to a memory stream:

```

``````

     ByteArrayOutputStream memoryStream = new ByteArrayOutputStream();
     // Create a new empty ISO archive
     try (IsoArchive isoArchive = new IsoArchive()) {
         // Add files to the ISO archive
         isoArchive.createEntry("example_file.txt", "path_to_file.txt");
         // Save the ISO archive to a memory stream
         isoArchive.save(memoryStream);
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | java.io.OutputStream | поток, в который будет сохранён образ ISO |
| saveOptions | [IsoSaveOptions](../../com.aspose.zip/isosaveoptions) | параметры, с которыми сохраняется ISO-архив |

### save(String path) {#save-java.lang.String-}
```
public final void save(String path)
```


Сохраняет ISO‑образ по указанному пути.

Следующий пример показывает, как сохранить ISO-архив в файл:

```

``````

// Создать новый пустой ISO‑архив
try (IsoArchive isoArchive = new IsoArchive()) {
// Добавить файлы в ISO‑архив
isoArchive.createEntry("example_file.txt", "path_to_file.txt");
// Сохранить ISO‑архив в файл
isoArchive.save("new_archive.iso");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path where the ISO image will be saved |

### save(String path, IsoSaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.IsoSaveOptions-}
```
public final void save(String path, IsoSaveOptions saveOptions)
```


Saves the ISO image to the specified path.

The following example shows how to save an ISO archive to a file:

```

``````

     // Create a new empty ISO archive
     try (IsoArchive isoArchive = new IsoArchive()) {
         // Add files to the ISO archive
         isoArchive.createEntry("example_file.txt", "path_to_file.txt");
         // Save the ISO archive to a file
         isoArchive.save("new_archive.iso");
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| path | java.lang.String | путь, по которому будет сохранён образ ISO |
| saveOptions | [IsoSaveOptions](../../com.aspose.zip/isosaveoptions) | параметры, с которыми сохраняется ISO-архив |

