---
title: "LzmaArchive"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Этот класс представляет файл архива LZMA."
type: docs
weight: 86
url: /ru/java/com.aspose.zip/lzmaarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class LzmaArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

Этот класс представляет файл архива LZMA. Используйте его для создания или извлечения архивов LZMA.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [LzmaArchive()](#LzmaArchive--) | Инициализирует новый экземпляр класса [LzmaArchive](../../com.aspose.zip/lzmaarchive) и создает архив в формате lzma. |
| [LzmaArchive(LzmaArchiveSettings settings)](#LzmaArchive-com.aspose.zip.LzmaArchiveSettings-) | Инициализирует новый экземпляр класса [LzmaArchive](../../com.aspose.zip/lzmaarchive) и создает архив в формате lzma. |
| [LzmaArchive(InputStream source)](#LzmaArchive-java.io.InputStream-) | Инициализирует новый экземпляр класса [LzmaArchive](../../com.aspose.zip/lzmaarchive), подготовленный для распаковки. |
| [LzmaArchive(String path)](#LzmaArchive-java.lang.String-) | Инициализирует новый экземпляр класса [LzmaArchive](../../com.aspose.zip/lzmaarchive), подготовленный для распаковки. |
## Методы

| Метод | Описание |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | Извлекает архив lzma в файл. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Извлекает архив lzma в поток. |
| [extract(String path)](#extract-java.lang.String-) | Извлекает архив lzma в файл по пути. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Извлекает содержимое архива в указанную директорию. |
| [getFileEntries()](#getFileEntries--) | Получает элементы типа [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), составляющие архив lzma. |
| [getFormat()](#getFormat--) | Получает формат архива. |
| [getLength()](#getLength--) | Получает длину. |
| [getName()](#getName--) | Имя оригинального файла. |
| [save(File destination)](#save-java.io.File-) | Сохраняет архив lzma в указанный файл назначения. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Сохраняет lzma-архив в предоставленный поток. |
| [save(String destinationFileName)](#save-java.lang.String-) | Сохраняет архив lzma в указанный файл назначения. |
| [setSource(File file)](#setSource-java.io.File-) | Устанавливает содержимое, которое будет сжато в архиве. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Устанавливает содержимое, которое будет сжато в архиве. |
| [setSource(String sourcePath)](#setSource-java.lang.String-) | Устанавливает содержимое, которое будет сжато в архиве. |
### LzmaArchive() {#LzmaArchive--}
```
public LzmaArchive()
```


Инициализирует новый экземпляр класса [LzmaArchive](../../com.aspose.zip/lzmaarchive) и создает архив в формате lzma.

### LzmaArchive(LzmaArchiveSettings settings) {#LzmaArchive-com.aspose.zip.LzmaArchiveSettings-}
```
public LzmaArchive(LzmaArchiveSettings settings)
```


Инициализирует новый экземпляр класса [LzmaArchive](../../com.aspose.zip/lzmaarchive) и создает архив в формате lzma.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| settings | [LzmaArchiveSettings](../../com.aspose.zip/lzmaarchivesettings) | набор настроек конкретного lzma-архива |

### LzmaArchive(InputStream source) {#LzmaArchive-java.io.InputStream-}
```
public LzmaArchive(InputStream source)
```


Инициализирует новый экземпляр класса [LzmaArchive](../../com.aspose.zip/lzmaarchive), подготовленный для распаковки.

Этот конструктор не выполняет распаковку. См. метод [extract(OutputStream)](../../com.aspose.zip/lzmaarchive\#extract-OutputStream-) для распаковки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| source | java.io.InputStream | источник архива |

### LzmaArchive(String path) {#LzmaArchive-java.lang.String-}
```
public LzmaArchive(String path)
```


Инициализирует новый экземпляр класса [LzmaArchive](../../com.aspose.zip/lzmaarchive), подготовленный для распаковки.

```

``````

try (FileInputStream sourceLzmaFile = new FileInputStream(sourceFileName)) {
try (FileOutputStream extractedFile = new FileOutputStream(extractedFileName)) {
try (LzmaArchive archive = new LzmaArchive(sourceLzmaFile)) {
archive.extract(extractedFile);
}
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [extract(OutputStream)](../../com.aspose.zip/lzmaarchive\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the source of the archive |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Extracts lzma archive to a file.

```

``````

     try (FileInputStream lzmaFile = new FileInputStream(sourceFileName)) {
         try (LzmaArchive archive = new LzmaArchive(lzmaFile)) {
             archive.extract(new File("extracted.bin"));
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| file | java.io.File | файл для хранения распакованных данных |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Извлекает архив lzma в поток.

```

``````

try (FileInputStream sourceLzmaFile = new FileInputStream(sourceFileName)) {
try (FileOutputStream extractedFile = new FileOutputStream(extractedFileName)) {
try (LzmaArchive archive = new LzmaArchive(sourceLzmaFile)) {
archive.extract(extractedFile);
}
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | the stream for storing decompressed data |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts lzma archive to a file by path.

```

``````

     try (FileInputStream lzmaFile = new FileInputStream(sourceFileName)) {
         try (LzmaArchive archive = new LzmaArchive(lzmaFile)) {
             archive.extract("extracted.bin");
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| path | java.lang.String | путь к файлу, в котором будут храниться распакованные данные |

**Returns:**
java.io.File — информация о извлечённом файле
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Извлекает содержимое архива в указанную директорию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | destinationDirectory | java.lang.String | путь к каталогу, в который будут помещены извлечённые файлы. |

Если каталог не существует, он будет создан |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Получает элементы типа [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), составляющие архив lzma.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - элементы типа [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), составляющие lzma-архив.
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Получает формат архива.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getLength() {#getLength--}
```
public final Long getLength()
```


Получает длину.

**Returns:**
java.lang.Long - длина
### getName() {#getName--}
```
public final String getName()
```


Имя оригинального файла.

**Returns:**
java.lang.String - имя оригинального файла
### save(File destination) {#save-java.io.File-}
```
public final void save(File destination)
```


Сохраняет архив lzma в указанный файл назначения.

```

``````

try (LzmaArchive archive = new LzmaArchive()) {
archive.setSource(new File("data.bin"));
archive.save(new File("archive.lzma"));
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.File | the file, which will be opened as destination stream |

### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves lzma archive to the stream provided.

```

``````

     try (FileOutputStream lzmaFile = new FileOutputStream("archive.lzma")) {
         try (LzmaArchive archive = new LzmaArchive()) {
             archive.setSource("data.bin");
             archive.save(lzmaFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
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


Сохраняет архив lzma в указанный файл назначения.

```

``````

try (LzmaArchive archive = new LzmaArchive()) {
archive.setSource(new File("data.bin"));
archive.save("result.lzma");
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

     try (LzmaArchive archive = new LzmaArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.lzma");
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

try (LzmaArchive archive = new LzmaArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] { 0x00, (byte) 0xFF }));
archive.save("archive.lzma");
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

     try (LzmaArchive archive = new LzmaArchive()) {
         archive.setSource("data.bin");
         archive.save("archive.lzma");
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourcePath | java.lang.String | путь к файлу, который будет открыт как входной поток |

