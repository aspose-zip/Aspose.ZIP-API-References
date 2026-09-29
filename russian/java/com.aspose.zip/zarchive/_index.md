---
title: "ZArchive"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Этот класс представляет файл архива Z compress."
type: docs
weight: 153
url: /ru/java/com.aspose.zip/zarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), [com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class ZArchive implements IArchiveFileEntry, IArchive, AutoCloseable
```

Этот класс представляет файл архива Z (compress). Используйте его для создания или извлечения архивов Z.

Смотрите [Z Compressed File Format ][Z Compressed File Format]


[Z Compressed File Format]: https://docs.fileformat.com/compression/z/
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [ZArchive()](#ZArchive--) | Инициализирует новый экземпляр класса [ZArchive](../../com.aspose.zip/zarchive), подготовленного для сжатия. |
| [ZArchive(InputStream source)](#ZArchive-java.io.InputStream-) | Инициализирует новый экземпляр класса [ZArchive](../../com.aspose.zip/zarchive), подготовленного для распаковки. |
| [ZArchive(InputStream source, ZArchiveLoadOptions loadOptions)](#ZArchive-java.io.InputStream-com.aspose.zip.ZArchiveLoadOptions-) | Инициализирует новый экземпляр класса [ZArchive](../../com.aspose.zip/zarchive), подготовленного для распаковки. |
| [ZArchive(String path)](#ZArchive-java.lang.String-) | Инициализирует новый экземпляр класса [ZArchive](../../com.aspose.zip/zarchive), подготовленного для распаковки. |
| [ZArchive(String path, ZArchiveLoadOptions loadOptions)](#ZArchive-java.lang.String-com.aspose.zip.ZArchiveLoadOptions-) | Инициализирует новый экземпляр класса [ZArchive](../../com.aspose.zip/zarchive), подготовленного для распаковки. |
## Методы

| Метод | Описание |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | Извлекает архив Z в файл. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Извлекает архив Z в поток. |
| [extract(String path)](#extract-java.lang.String-) | Извлекает архив Z в файл по пути. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Извлекает содержимое архива в указанную директорию. |
| [getFileEntries()](#getFileEntries--) | Возвращает записи типа [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), составляющие архив Z. |
| [getFormat()](#getFormat--) | Получает формат архива. |
| [getLength()](#getLength--) | Получает длину записи в байтах. |
| [getName()](#getName--) | Возвращает имя записи в архиве. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Сохраняет архив Z в предоставленный поток. |
| [save(OutputStream output, ZArchiveSaveOptions settings)](#save-java.io.OutputStream-com.aspose.zip.ZArchiveSaveOptions-) | Сохраняет архив Z в предоставленный поток. |
| [save(String destinationFileName)](#save-java.lang.String-) | Сохраняет Z-архив в указанный файл назначения. |
| [save(String destinationFileName, ZArchiveSaveOptions settings)](#save-java.lang.String-com.aspose.zip.ZArchiveSaveOptions-) | Сохраняет Z-архив в указанный файл назначения. |
| [setSource(File file)](#setSource-java.io.File-) | Устанавливает содержимое, которое будет сжато в архиве. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Устанавливает содержимое, которое будет сжато в архиве. |
| [setSource(String sourcePath)](#setSource-java.lang.String-) | Устанавливает содержимое, которое будет сжато в архиве. |
### ZArchive() {#ZArchive--}
```
public ZArchive()
```


Инициализирует новый экземпляр класса [ZArchive](../../com.aspose.zip/zarchive), подготовленного для сжатия.

### ZArchive(InputStream source) {#ZArchive-java.io.InputStream-}
```
public ZArchive(InputStream source)
```


Инициализирует новый экземпляр класса [ZArchive](../../com.aspose.zip/zarchive), подготовленного для распаковки.

Этот конструктор не распаковывает. Смотрите метод [extract(OutputStream)](../../com.aspose.zip/zarchive\#extract-OutputStream-) для распаковки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| source | java.io.InputStream | источник архива |

### ZArchive(InputStream source, ZArchiveLoadOptions loadOptions) {#ZArchive-java.io.InputStream-com.aspose.zip.ZArchiveLoadOptions-}
```
public ZArchive(InputStream source, ZArchiveLoadOptions loadOptions)
```


Инициализирует новый экземпляр класса [ZArchive](../../com.aspose.zip/zarchive), подготовленного для распаковки.

Этот конструктор не распаковывает. Смотрите метод [extract(OutputStream)](../../com.aspose.zip/zarchive\#extract-OutputStream-) для распаковки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| source | java.io.InputStream | источник архива |
| loadOptions | [ZArchiveLoadOptions](../../com.aspose.zip/zarchiveloadoptions) | параметры загрузки архива |

### ZArchive(String path) {#ZArchive-java.lang.String-}
```
public ZArchive(String path)
```


Инициализирует новый экземпляр класса [ZArchive](../../com.aspose.zip/zarchive), подготовленного для распаковки.

Этот конструктор не распаковывает. Смотрите метод [extract(String)](../../com.aspose.zip/zarchive\#extract-String-) для распаковки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| path | java.lang.String | путь к источнику архива |

### ZArchive(String path, ZArchiveLoadOptions loadOptions) {#ZArchive-java.lang.String-com.aspose.zip.ZArchiveLoadOptions-}
```
public ZArchive(String path, ZArchiveLoadOptions loadOptions)
```


Инициализирует новый экземпляр класса [ZArchive](../../com.aspose.zip/zarchive), подготовленного для распаковки.

Этот конструктор не распаковывает. Смотрите метод [extract(String)](../../com.aspose.zip/zarchive\#extract-String-) для распаковки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| path | java.lang.String | путь к источнику архива |
| loadOptions | [ZArchiveLoadOptions](../../com.aspose.zip/zarchiveloadoptions) | параметры загрузки архива |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Извлекает архив Z в файл.

```

``````

try (FileInputStream zFile = new FileInputStream(\"sourceFileName\")) {
try (ZArchive archive = new ZArchive(zFile)) {
archive.extract(new File("extracted.bin"));
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | the file for storing decompressed data |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts Z archive to a stream.

```

``````

     try (FileInputStream zFile = new FileInputStream("sourceFileName")) {
         try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
             try (ZArchive archive = new ZArchive(zFile)) {
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


Извлекает архив Z в файл по пути.

```

``````

try (FileInputStream zFile = new FileInputStream(\"sourceFileName\")) {
try (ZArchive archive = new ZArchive(zFile)) {
archive.extract("extracted.bin");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to file which will store decompressed data |

**Returns:**
java.io.File - the file info of the extracted file
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts content of the archive to the directory provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in

If the directory does not exist, it will be created. |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the Z archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the Z archive
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
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves Z archive to the stream provided.

```

``````

     try (FileOutputStream zFile = new FileOutputStream("data.bin.Z")) {
         try (ZArchive archive = new ZArchive()) {
             archive.setSource("data.bin");
             archive.save(zFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| output | java.io.OutputStream | поток назначения |

### save(OutputStream output, ZArchiveSaveOptions settings) {#save-java.io.OutputStream-com.aspose.zip.ZArchiveSaveOptions-}
```
public final void save(OutputStream output, ZArchiveSaveOptions settings)
```


Сохраняет архив Z в предоставленный поток.

```

``````

try (FileOutputStream zFile = new FileOutputStream(\"data.bin.Z\")) {
try (ZArchive archive = new ZArchive()) {
archive.setSource("data.bin");
archive.save(zFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | the destination stream |
| settings | [ZArchiveSaveOptions](../../com.aspose.zip/zarchivesaveoptions) | the settings for archive composition |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves Z archive to the destination file provided.

```

``````

     try (ZArchive archive = new ZArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("data.bin.Z");
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| destinationFileName | java.lang.String | путь к создаваемому архиву. Если указанный файл уже существует, он будет перезаписан |

### save(String destinationFileName, ZArchiveSaveOptions settings) {#save-java.lang.String-com.aspose.zip.ZArchiveSaveOptions-}
```
public final void save(String destinationFileName, ZArchiveSaveOptions settings)
```


Сохраняет Z-архив в указанный файл назначения.

```

``````

try (ZArchive archive = new ZArchive()) {
archive.setSource(new File("data.bin"));
archive.save(\"data.bin.Z\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| settings | [ZArchiveSaveOptions](../../com.aspose.zip/zarchivesaveoptions) | the settings for archive composition |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Sets the content to be compressed within the archive.

```

``````

     try (ZArchive archive = new ZArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("data.bin.Z");
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| file | java.io.File | информация о файле, который будет открыт как входной поток |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Устанавливает содержимое, которое будет сжато в архиве.

```

``````

try (ZArchive archive = new ZArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] {
0x00,
(byte) 0xFF
}));
archive.save(\"archive.Z\");
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

     try (ZArchive archive = new ZArchive()) {
         archive.setSource("data.bin");
         archive.save("data.bin.Z");
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourcePath | java.lang.String | путь к файлу, который будет открыт как входной поток |

