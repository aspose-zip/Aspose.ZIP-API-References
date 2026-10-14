---
title: "AlzArchive"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Представляет файл архива ALZ."
type: docs
weight: 11
url: /ru/java/com.aspose.zip/alzarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class AlzArchive implements IArchive, AutoCloseable
```

Представляет файл архива ALZ. Используйте этот класс для просмотра и извлечения архивов ALZ.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [AlzArchive(InputStream stream)](#AlzArchive-java.io.InputStream-) | Инициализирует архив ALZ из потока. |
| [AlzArchive(InputStream stream, AlzArchiveLoadOptions loadOptions)](#AlzArchive-java.io.InputStream-com.aspose.zip.AlzArchiveLoadOptions-) | Инициализирует архив ALZ из потока, используя предоставленные параметры загрузки. |
| [AlzArchive(String filePath)](#AlzArchive-java.lang.String-) | Инициализирует архив ALZ из пути к файлу. |
| [AlzArchive(String filePath, AlzArchiveLoadOptions loadOptions)](#AlzArchive-java.lang.String-com.aspose.zip.AlzArchiveLoadOptions-) | Инициализирует архив ALZ из пути к файлу, используя предоставленные параметры загрузки. |
## Методы

| Метод | Описание |
| --- | --- |
| [close()](#close--) | Освобождает ресурсы, удерживаемые этим архивом. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Извлекает все файлы и каталоги в указанный каталог. |
| [getEntries()](#getEntries--) | Получает элементы, составляющие этот архив. |
| [getFileEntries()](#getFileEntries--) | Получает элементы через общий интерфейс архива. |
| [getFormat()](#getFormat--) | Получает формат архива. |
### AlzArchive(InputStream stream) {#AlzArchive-java.io.InputStream-}
```
public AlzArchive(InputStream stream)
```


Инициализирует архив ALZ из потока.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | java.io.InputStream | Поток архива ALZ; он должен поддерживать чтение и перемещение. |

### AlzArchive(InputStream stream, AlzArchiveLoadOptions loadOptions) {#AlzArchive-java.io.InputStream-com.aspose.zip.AlzArchiveLoadOptions-}
```
public AlzArchive(InputStream stream, AlzArchiveLoadOptions loadOptions)
```


Инициализирует архив ALZ из потока, используя предоставленные параметры загрузки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | java.io.InputStream | Поток архива ALZ; он должен поддерживать чтение и перемещение. |
| loadOptions | [AlzArchiveLoadOptions](../../com.aspose.zip/alzarchiveloadoptions) | параметры, используемые для загрузки архива |

### AlzArchive(String filePath) {#AlzArchive-java.lang.String-}
```
public AlzArchive(String filePath)
```


Инициализирует архив ALZ из пути к файлу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| filePath | java.lang.String | путь к архиву ALZ |

### AlzArchive(String filePath, AlzArchiveLoadOptions loadOptions) {#AlzArchive-java.lang.String-com.aspose.zip.AlzArchiveLoadOptions-}
```
public AlzArchive(String filePath, AlzArchiveLoadOptions loadOptions)
```


Инициализирует архив ALZ из пути к файлу, используя предоставленные параметры загрузки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| filePath | java.lang.String | путь к архиву ALZ |
| loadOptions | [AlzArchiveLoadOptions](../../com.aspose.zip/alzarchiveloadoptions) | параметры, используемые для загрузки архива |

### close() {#close--}
```
public void close()
```


Освобождает ресурсы, удерживаемые этим архивом.

### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Извлекает все файлы и каталоги в указанный каталог.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| destinationDirectory | java.lang.String | каталог назначения; он создаётся при необходимости |

### getEntries() {#getEntries--}
```
public final List<AlzEntry> getEntries()
```


Получает элементы, составляющие этот архив.

**Returns:**
java.util.List&lt;com.aspose.zip.AlzEntry&gt; - неизменяемый список записей ALZ
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Получает элементы через общий интерфейс архива.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - записи архива
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Получает формат архива.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - [ArchiveFormat.Alz](../../com.aspose.zip/archiveformat\#Alz)
