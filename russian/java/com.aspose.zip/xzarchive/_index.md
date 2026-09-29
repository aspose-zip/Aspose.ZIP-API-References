---
title: "XzArchive"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Этот класс представляет файл архива xz."
type: docs
weight: 146
url: /ru/java/com.aspose.zip/xzarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), [com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class XzArchive implements IArchiveFileEntry, IArchive, AutoCloseable
```

Этот класс представляет файл архива xz. Используйте его для создания и извлечения архивов xz.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [XzArchive()](#XzArchive--) | Инициализирует новый экземпляр класса [XzArchive](../../com.aspose.zip/xzarchive) и создает архив в формате xz. |
| [XzArchive(XzArchiveSettings settings)](#XzArchive-com.aspose.zip.XzArchiveSettings-) | Инициализирует новый экземпляр класса [XzArchive](../../com.aspose.zip/xzarchive) и создает архив в формате xz. |
| [XzArchive(InputStream source)](#XzArchive-java.io.InputStream-) | Инициализирует новый экземпляр класса [XzArchive](../../com.aspose.zip/xzarchive), подготовленный для распаковки. |
| [XzArchive(InputStream source, XzLoadOptions options)](#XzArchive-java.io.InputStream-com.aspose.zip.XzLoadOptions-) | Инициализирует новый экземпляр класса [XzArchive](../../com.aspose.zip/xzarchive), подготовленный для распаковки. |
| [XzArchive(String path)](#XzArchive-java.lang.String-) | Инициализирует новый экземпляр класса [XzArchive](../../com.aspose.zip/xzarchive), подготовленный для распаковки. |
| [XzArchive(String path, XzLoadOptions options)](#XzArchive-java.lang.String-com.aspose.zip.XzLoadOptions-) | Инициализирует новый экземпляр класса [XzArchive](../../com.aspose.zip/xzarchive), подготовленный для распаковки. |
## Методы

| Метод | Описание |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | Извлекает архив xz в файл. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Извлекает архив xz в поток. |
| [extract(String path)](#extract-java.lang.String-) | Извлекает архив xz в файл по пути. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Извлекает содержимое архива в указанную директорию. |
| [getFileEntries()](#getFileEntries--) | Получает записи типа [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), составляющие xz-архив. |
| [getFormat()](#getFormat--) | Получает формат архива. |
| [getLength()](#getLength--) | Получает длину записи в байтах. |
| [getName()](#getName--) | Возвращает имя записи в архиве. |
| [getUncompressedSize()](#getUncompressedSize--) | Получает несжатый размер данных файла в байтах. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Сохраняет xz-архив в предоставленный поток. |
| [save(String destinationFileName)](#save-java.lang.String-) | Сохраняет xz-архив в указанный файл назначения. |
| [setSource(File file)](#setSource-java.io.File-) | Устанавливает содержимое, которое будет сжато в архиве. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Устанавливает содержимое, которое будет сжато в архиве. |
| [setSource(String sourcePath)](#setSource-java.lang.String-) | Устанавливает содержимое, которое будет сжато в архиве. |
### XzArchive() {#XzArchive--}
```
public XzArchive()
```


Инициализирует новый экземпляр класса [XzArchive](../../com.aspose.zip/xzarchive) и создает архив в формате xz.

### XzArchive(XzArchiveSettings settings) {#XzArchive-com.aspose.zip.XzArchiveSettings-}
```
public XzArchive(XzArchiveSettings settings)
```


Инициализирует новый экземпляр класса [XzArchive](../../com.aspose.zip/xzarchive) и создает архив в формате xz.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| settings | [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) | набор параметров конкретного xz-архива: размер словаря, размер блока, тип проверки |

### XzArchive(InputStream source) {#XzArchive-java.io.InputStream-}
```
public XzArchive(InputStream source)
```


Инициализирует новый экземпляр класса [XzArchive](../../com.aspose.zip/xzarchive), подготовленный для распаковки.

Этот конструктор не выполняет распаковку. См. метод [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\#extract-java.io.OutputStream-) для распаковки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| source | java.io.InputStream | источник архива |

### XzArchive(InputStream source, XzLoadOptions options) {#XzArchive-java.io.InputStream-com.aspose.zip.XzLoadOptions-}
```
public XzArchive(InputStream source, XzLoadOptions options)
```


Инициализирует новый экземпляр класса [XzArchive](../../com.aspose.zip/xzarchive), подготовленный для распаковки.

Этот конструктор не выполняет распаковку. См. метод [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\#extract-java.io.OutputStream-) для распаковки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| source | java.io.InputStream | источник архива |
| options | [XzLoadOptions](../../com.aspose.zip/xzloadoptions) | Параметры загрузки архива. |

### XzArchive(String path) {#XzArchive-java.lang.String-}
```
public XzArchive(String path)
```


Инициализирует новый экземпляр класса [XzArchive](../../com.aspose.zip/xzarchive), подготовленный для распаковки.

Этот конструктор не выполняет распаковку. См. метод [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\#extract-java.io.OutputStream-) для распаковки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| path | java.lang.String | путь к источнику архива |

### XzArchive(String path, XzLoadOptions options) {#XzArchive-java.lang.String-com.aspose.zip.XzLoadOptions-}
```
public XzArchive(String path, XzLoadOptions options)
```


Инициализирует новый экземпляр класса [XzArchive](../../com.aspose.zip/xzarchive), подготовленный для распаковки.

Этот конструктор не выполняет распаковку. См. метод [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\#extract-java.io.OutputStream-) для распаковки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| path | java.lang.String | путь к источнику архива |
| options | [XzLoadOptions](../../com.aspose.zip/xzloadoptions) |  |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Извлекает архив xz в файл.

```

``````

try (FileInputStream xzFile = new FileInputStream("sourceFileName")) {
try (XzArchive archive = new XzArchive(xzFile)) {
archive.extract(new File("extracted.bin"));
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | file for storing decompressed data |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts xz archive to a stream.

```

``````

     try (FileInputStream xzFile = new FileInputStream("sourceFileName")) {
         try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
             try (XzArchive archive = new XzArchive(xzFile)) {
                 archive.extract(extractedFile);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| назначение | java.io.OutputStream | поток для хранения распакованных данных |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Извлекает архив xz в файл по пути.

```

``````

try (FileInputStream xzFile = new FileInputStream("sourceFileName")) {
try (XzArchive archive = new XzArchive(xzFile)) {
archive.extract("extracted.bin");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | path to file which will store decompressed data |

**Returns:**
java.io.File - java.io.File instance containing extracted data
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts content of the archive to the directory provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in.

If the directory does not exist, it will be created. |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the xz archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the xz archive
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Gets the archive format.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets the length of the entry in bytes.

**Returns:**
java.lang.Long - the length of the entry in bytes
### getName() {#getName--}
```
public final String getName()
```


Gets the name of the entry within archive.

**Returns:**
java.lang.String - the name of the entry within archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets the uncompressed size of the file data in bytes.

**Returns:**
long - the uncompressed size of the file data in bytes
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves xz archive to the stream provided.

```

``````

     try (FileOutputStream xzFile = new FileOutputStream("archive.xz")) {
         try (XzArchive archive = new XzArchive()) {
             archive.setSource("data.bin");
             archive.save(xzFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| output | java.io.OutputStream | поток назначения |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Сохраняет xz-архив в указанный файл назначения.

```

``````

try (XzArchive archive = new XzArchive()) {
archive.setSource(new File("data.bin"));
archive.save("result.xz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Sets the content to be compressed within the archive.

```

``````

     try (XzArchive archive = new XzArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.xz");
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| file | java.io.File | файл, который будет открыт как входной поток |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Устанавливает содержимое, которое будет сжато в архиве.

```

``````

try (XzArchive archive = new XzArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] { 0x00, (byte) 0xFF }));
archive.save("archive.xz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | the input stream for the archive |

### setSource(String sourcePath) {#setSource-java.lang.String-}
```
public final void setSource(String sourcePath)
```


Sets the content to be compressed within the archive.

```

``````

     try (XzArchive archive = new XzArchive()) {
         archive.setSource("data.bin");
         archive.save("archive.xz");
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourcePath | java.lang.String | путь к файлу, который будет открыт как входной поток |

