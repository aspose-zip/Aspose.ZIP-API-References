---
title: "AppleArchive"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Этот класс представляет файл Apple Archive .aar."
type: docs
weight: 16
url: /ru/java/com.aspose.zip/applearchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class AppleArchive implements IArchive, AutoCloseable
```

Этот класс представляет файл Apple Archive (.aar). Используйте его для создания файлов Apple Archive.

Apple и Apple Archive являются товарными знаками компании Apple Inc.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [AppleArchive()](#AppleArchive--) | Инициализирует новый экземпляр класса [AppleArchive](../../com.aspose.zip/applearchive) с настройками, используемыми для составленных записей. |
| [AppleArchive(AppleArchiveEntrySettings newEntrySettings)](#AppleArchive-com.aspose.zip.AppleArchiveEntrySettings-) | Инициализирует новый экземпляр класса [AppleArchive](../../com.aspose.zip/applearchive) с настройками, используемыми для составленных записей. |
| [AppleArchive(InputStream sourceStream)](#AppleArchive-java.io.InputStream-) | Инициализирует новый экземпляр класса [AppleArchive](../../com.aspose.zip/applearchive) и формирует список записей, который может быть извлечён из архива. |
| [AppleArchive(InputStream sourceStream, AppleArchiveLoadOptions loadOptions)](#AppleArchive-java.io.InputStream-com.aspose.zip.AppleArchiveLoadOptions-) | Инициализирует новый экземпляр класса [AppleArchive](../../com.aspose.zip/applearchive) и формирует список записей, который может быть извлечён из архива. |
| [AppleArchive(String path)](#AppleArchive-java.lang.String-) | Инициализирует новый экземпляр класса [AppleArchive](../../com.aspose.zip/applearchive) и формирует список записей, который может быть извлечён из архива. |
| [AppleArchive(String path, AppleArchiveLoadOptions loadOptions)](#AppleArchive-java.lang.String-com.aspose.zip.AppleArchiveLoadOptions-) | Инициализирует новый экземпляр класса [AppleArchive](../../com.aspose.zip/applearchive) и формирует список записей, который может быть извлечён из архива. |
## Методы

| Метод | Описание |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога. |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога. |
| [createEntry(String name, File fileInfo)](#createEntry-java.lang.String-java.io.File-) | Создаёт одну запись внутри архива. |
| [createEntry(String name, File fileInfo, boolean openImmediately)](#createEntry-java.lang.String-java.io.File-boolean-) | Создаёт одну запись внутри архива. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | Создаёт одну запись внутри архива. |
| [createEntry(String name, String path)](#createEntry-java.lang.String-java.lang.String-) | Создаёт одну запись внутри архива. |
| [createEntry(String name, String path, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | Создаёт одну запись внутри архива. |
| [dispose()](#dispose--) | Выполняет определённые приложением задачи, связанные с освобождением, высвобождением или сбросом неуправляемых ресурсов. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Извлекает все файлы из архива в указанный каталог. |
| [getEntries()](#getEntries--) | Получает записи, составляющие архив. |
| [getFileEntries()](#getFileEntries--) | Получает записи типа [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), составляющие архив. |
| [getFormat()](#getFormat--) | Получает формат архива. |
| [getNewEntrySettings()](#getNewEntrySettings--) | Получает настройки, используемые для новых составленных записей. |
| [isSolid()](#isSolid--) | Возвращает значение, указывающее, использует ли архив сплошное сжатие. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Сохраняет архив в предоставленный поток. |
| [save(String destinationFileName)](#save-java.lang.String-) | Сохраняет архив в указанный файл назначения. |
### AppleArchive() {#AppleArchive--}
```
public AppleArchive()
```


Инициализирует новый экземпляр класса [AppleArchive](../../com.aspose.zip/applearchive) с настройками, используемыми для составленных записей.

### AppleArchive(AppleArchiveEntrySettings newEntrySettings) {#AppleArchive-com.aspose.zip.AppleArchiveEntrySettings-}
```
public AppleArchive(AppleArchiveEntrySettings newEntrySettings)
```


Инициализирует новый экземпляр класса [AppleArchive](../../com.aspose.zip/applearchive) с настройками, используемыми для составленных записей.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| newEntrySettings | [AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings) | Настройки, используемые при создании нового Apple Archive. |

### AppleArchive(InputStream sourceStream) {#AppleArchive-java.io.InputStream-}
```
public AppleArchive(InputStream sourceStream)
```


Инициализирует новый экземпляр класса [AppleArchive](../../com.aspose.zip/applearchive) и формирует список записей, который может быть извлечён из архива.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | sourceStream | java.io.InputStream | Источник архива. |

Этот конструктор не распаковывает ни одну запись. См. методы [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) и [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) для распаковки. |

### AppleArchive(InputStream sourceStream, AppleArchiveLoadOptions loadOptions) {#AppleArchive-java.io.InputStream-com.aspose.zip.AppleArchiveLoadOptions-}
```
public AppleArchive(InputStream sourceStream, AppleArchiveLoadOptions loadOptions)
```


Инициализирует новый экземпляр класса [AppleArchive](../../com.aspose.zip/applearchive) и формирует список записей, который может быть извлечён из архива.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceStream | java.io.InputStream | Источник архива. |
|  | loadOptions | [AppleArchiveLoadOptions](../../com.aspose.zip/applearchiveloadoptions) | Параметры для загрузки существующего архива. |

Этот конструктор не распаковывает ни одну запись. См. методы [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) и [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) для распаковки. |

### AppleArchive(String path) {#AppleArchive-java.lang.String-}
```
public AppleArchive(String path)
```


Инициализирует новый экземпляр класса [AppleArchive](../../com.aspose.zip/applearchive) и формирует список записей, который может быть извлечён из архива.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | path | java.lang.String | Полный или относительный путь к файлу архива. |

Этот конструктор не распаковывает ни одну запись. См. методы [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) и [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) для распаковки. |

### AppleArchive(String path, AppleArchiveLoadOptions loadOptions) {#AppleArchive-java.lang.String-com.aspose.zip.AppleArchiveLoadOptions-}
```
public AppleArchive(String path, AppleArchiveLoadOptions loadOptions)
```


Инициализирует новый экземпляр класса [AppleArchive](../../com.aspose.zip/applearchive) и формирует список записей, который может быть извлечён из архива.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| path | java.lang.String | Полный или относительный путь к файлу архива. |
|  | loadOptions | [AppleArchiveLoadOptions](../../com.aspose.zip/applearchiveloadoptions) | Параметры для загрузки существующего архива. |

Этот конструктор не распаковывает ни одну запись. См. методы [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) и [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) для распаковки. |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final AppleArchive createEntries(File directory)
```


Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| directory | java.io.File | Каталог для сжатия. |

**Returns:**
[AppleArchive](../../com.aspose.zip/applearchive) - The archive with entries composed.
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final AppleArchive createEntries(File directory, boolean includeRootDirectory)
```


Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| directory | java.io.File | Каталог для сжатия. |
| includeRootDirectory | boolean | Указывает, следует ли включать сам корневой каталог или нет. |

**Returns:**
[AppleArchive](../../com.aspose.zip/applearchive) - The archive with entries composed.
### createEntry(String name, File fileInfo) {#createEntry-java.lang.String-java.io.File-}
```
public final AppleArchiveEntry createEntry(String name, File fileInfo)
```


Создаёт одну запись внутри архива.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| имя | java.lang.String | Имя записи. |
| fileInfo | java.io.File | Метаданные файла, который будет сжат. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, File fileInfo, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final AppleArchiveEntry createEntry(String name, File fileInfo, boolean openImmediately)
```


Создаёт одну запись внутри архива.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| имя | java.lang.String | Имя записи. |
| fileInfo | java.io.File | Метаданные файла, который будет сжат. |
| openImmediately | boolean | True, если файл открывается сразу, иначе файл открывается при сохранении архива. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final AppleArchiveEntry createEntry(String name, InputStream source)
```


Создаёт одну запись внутри архива.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| имя | java.lang.String | Имя записи. |
| source | java.io.InputStream | Входной поток для элемента. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, String path) {#createEntry-java.lang.String-java.lang.String-}
```
public final AppleArchiveEntry createEntry(String name, String path)
```


Создаёт одну запись внутри архива.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| имя | java.lang.String | Имя записи. |
| path | java.lang.String | Путь к файлу для сжатия. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, String path, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final AppleArchiveEntry createEntry(String name, String path, boolean openImmediately)
```


Создаёт одну запись внутри архива.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| имя | java.lang.String | Имя записи. |
| path | java.lang.String | Путь к файлу для сжатия. |
| openImmediately | boolean | True, если файл открывается сразу, иначе файл открывается при сохранении архива. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### dispose() {#dispose--}
```
public final void dispose()
```


Выполняет определённые приложением задачи, связанные с освобождением, высвобождением или сбросом неуправляемых ресурсов.

### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Извлекает все файлы из архива в указанный каталог.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| destinationDirectory | java.lang.String | Путь к каталогу, в который будут помещены извлечённые файлы. |

### getEntries() {#getEntries--}
```
public final List<AppleArchiveEntry> getEntries()
```


Получает записи, составляющие архив.

**Returns:**
java.util.List&lt;com.aspose.zip.AppleArchiveEntry&gt; - записи, составляющие архив.
### getFileEntries() {#getFileEntries--}
```
public Iterable<IArchiveFileEntry> getFileEntries()
```


Получает записи типа [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), составляющие архив.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - записи типа [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), составляющие архив.
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Получает формат архива.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getNewEntrySettings() {#getNewEntrySettings--}
```
public final AppleArchiveEntrySettings getNewEntrySettings()
```


Получает настройки, используемые для новых составленных записей.

**Returns:**
[AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings) - settings used for newly composed entries.
### isSolid() {#isSolid--}
```
public final boolean isSolid()
```


Возвращает значение, указывающее, использует ли архив сплошное сжатие. В сплошном режиме все данные записей сжаты в один поток, и отдельное извлечение записей недоступно. Вместо этого используйте [IArchive.ExtractToDirectory()](../../com.aspose.zip/iarchive\#ExtractToDirectory--).

**Returns:**
boolean - значение, указывающее, использует ли архив сплошное сжатие.
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Сохраняет архив в предоставленный поток.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | output | java.io.OutputStream | Поток назначения. |

`output` должен быть доступен для записи. Некоторые настройки сжатия, такие как LZ4, также требуют поток с возможностью перемещения. |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Сохраняет архив в указанный файл назначения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| destinationFileName | java.lang.String | Путь к создаваемому архиву. |

