---
title: "WimArchive"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Этот класс представляет файл архива wim."
type: docs
weight: 130
url: /ru/java/com.aspose.zip/wimarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class WimArchive implements IArchive, AutoCloseable
```

Этот класс представляет файл архива wim.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [WimArchive(InputStream sourceStream)](#WimArchive-java.io.InputStream-) | Инициализирует новый экземпляр класса [WimArchive](../../com.aspose.zip/wimarchive) и формирует список записей, которые можно извлечь из архива. |
| [WimArchive(InputStream sourceStream, WimLoadOptions loadOptions)](#WimArchive-java.io.InputStream-com.aspose.zip.WimLoadOptions-) | Инициализирует новый экземпляр класса [WimArchive](../../com.aspose.zip/wimarchive) и формирует список записей, которые можно извлечь из архива. |
| [WimArchive(String path)](#WimArchive-java.lang.String-) | Инициализирует новый экземпляр класса [WimArchive](../../com.aspose.zip/wimarchive) и формирует список записей, которые можно извлечь из архива. |
| [WimArchive(String path, WimLoadOptions loadOptions)](#WimArchive-java.lang.String-com.aspose.zip.WimLoadOptions-) | Инициализирует новый экземпляр класса [WimArchive](../../com.aspose.zip/wimarchive) и формирует список записей, которые можно извлечь из архива. |
## Методы

| Метод | Описание |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Извлекает архив в файл по указанному пути. |
| [getBootImageIndex()](#getBootImageIndex--) | Получает (нумерацию с нуля) индекс загрузочного образа. |
| [getEntries()](#getEntries--) | Получает записи типа [WimEntry](../../com.aspose.zip/wimentry), составляющие архив. |
| [getFileEntries()](#getFileEntries--) | Получает записи типа [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), составляющие wim‑архив. |
| [getFileFormatVersion()](#getFileFormatVersion--) | Получает версию формата файла. |
| [getFormat()](#getFormat--) | Получает формат архива. |
| [getGuid()](#getGuid--) | Получает идентифицирующий UUID архива. |
| [getImages()](#getImages--) | Получает записи типа [WimImage](../../com.aspose.zip/wimimage), составляющие архив. |
| [getManifest()](#getManifest--) | Получает встроенный манифест, описывающий файл и содержащиеся в нём образы. |
### WimArchive(InputStream sourceStream) {#WimArchive-java.io.InputStream-}
```
public WimArchive(InputStream sourceStream)
```


Инициализирует новый экземпляр класса [WimArchive](../../com.aspose.zip/wimarchive) и формирует список записей, которые можно извлечь из архива.

Следующий пример показывает, как извлечь все записи в каталог.

```

``````

try (WimArchive archive = new WimArchive(new FileInputStream("archive.wim"))) {
archive.getImages().get_Item(0).extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry. See [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |

### WimArchive(InputStream sourceStream, WimLoadOptions loadOptions) {#WimArchive-java.io.InputStream-com.aspose.zip.WimLoadOptions-}
```
public WimArchive(InputStream sourceStream, WimLoadOptions loadOptions)
```


Initializes a new instance of the [WimArchive](../../com.aspose.zip/wimarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all of the entries to a directory.

```

``````

     try (WimArchive archive = new WimArchive(new FileInputStream("archive.wim"))) {
         archive.getImages().get_Item(0).extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

Этот конструктор не распаковывает ни одну запись. См. метод [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\#open--) для распаковки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceStream | java.io.InputStream | источник архива |
| loadOptions | [WimLoadOptions](../../com.aspose.zip/wimloadoptions) | Параметры для загрузки существующего архива. |

### WimArchive(String path) {#WimArchive-java.lang.String-}
```
public WimArchive(String path)
```


Инициализирует новый экземпляр класса [WimArchive](../../com.aspose.zip/wimarchive) и формирует список записей, которые можно извлечь из архива.

Следующий пример показывает, как извлечь все записи в каталог.

```

``````

try (WimArchive archive = new WimArchive("archive.wim")) {
archive.getImages().get_Item(0).extractToDirectory("C:\\extracted");
}
 
```

This constructor does not unpack any entry. See [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### WimArchive(String path, WimLoadOptions loadOptions) {#WimArchive-java.lang.String-com.aspose.zip.WimLoadOptions-}
```
public WimArchive(String path, WimLoadOptions loadOptions)
```


Initializes a new instance of the [WimArchive](../../com.aspose.zip/wimarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all of the entries to a directory.

```

``````

     try (WimArchive archive = new WimArchive("archive.wim")) {
         archive.getImages().get_Item(0).extractToDirectory("C:\\extracted");
     }
 
```

Этот конструктор не распаковывает ни одну запись. См. метод [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\#open--) для распаковки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| path | java.lang.String | путь к файлу архива |
| loadOptions | [WimLoadOptions](../../com.aspose.zip/wimloadoptions) | Параметры для загрузки существующего архива. |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Извлекает архив в файл по указанному пути.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| destinationDirectory | java.lang.String | путь к каталогу, в который будут помещены извлечённые файлы |

### getBootImageIndex() {#getBootImageIndex--}
```
public final int getBootImageIndex()
```


Получает (нумерацию с нуля) индекс загрузочного образа.

**Returns:**
int - (нумерацию с нуля) индекс загрузочного образа
### getEntries() {#getEntries--}
```
public final List<WimEntry> getEntries()
```


Получает записи типа [WimEntry](../../com.aspose.zip/wimentry), составляющие архив.

**Returns:**
java.util.List&lt;com.aspose.zip.WimEntry&gt; - записи, составляющие архив
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Получает записи типа [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), составляющие wim‑архив.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - записи типа [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), составляющие wim‑архив
### getFileFormatVersion() {#getFileFormatVersion--}
```
public final int getFileFormatVersion()
```


Получает версию формата файла.

**Returns:**
int - версия формата файла
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Получает формат архива.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getGuid() {#getGuid--}
```
public final UUID getGuid()
```


Получает идентифицирующий UUID архива.

**Returns:**
java.util.UUID - идентифицирующий UUID для архива
### getImages() {#getImages--}
```
public final List<WimImage> getImages()
```


Получает записи типа [WimImage](../../com.aspose.zip/wimimage), составляющие архив.

**Returns:**
java.util.List&lt;com.aspose.zip.WimImage&gt; - элементы типа [WimImage](../../com.aspose.zip/wimimage), составляющие архив
### getManifest() {#getManifest--}
```
public final String getManifest()
```


Получает встроенный манифест, описывающий файл и содержащиеся в нём образы.

**Returns:**
java.lang.String - встроенный манифест, описывающий файл и содержащиеся изображения
