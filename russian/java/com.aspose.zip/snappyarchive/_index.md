---
title: "SnappyArchive"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Этот класс представляет файл архива snappy."
type: docs
weight: 121
url: /ru/java/com.aspose.zip/snappyarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class SnappyArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

Этот класс представляет файл snappy‑архива. Используйте его для создания или извлечения snappy‑архивов.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [SnappyArchive()](#SnappyArchive--) | Инициализирует новый экземпляр класса [SnappyArchive](../../com.aspose.zip/snappyarchive), подготовленный для сжатия. |
| [SnappyArchive(InputStream source)](#SnappyArchive-java.io.InputStream-) | Инициализирует новый экземпляр класса [SnappyArchive](../../com.aspose.zip/snappyarchive), подготовленный для распаковки. |
| [SnappyArchive(String path)](#SnappyArchive-java.lang.String-) | Инициализирует новый экземпляр класса [SnappyArchive](../../com.aspose.zip/snappyarchive), подготовленный для распаковки. |
## Методы

| Метод | Описание |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | Извлекает snappy‑архив в файл. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Извлекает snappy‑архив в поток. |
| [extract(String path)](#extract-java.lang.String-) | Извлекает snappy‑архив в файл по пути. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Извлекает содержимое архива в указанную директорию. |
| [getFileEntries()](#getFileEntries--) | Возвращает элементы типа [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), составляющие snappy‑архив. |
| [getFormat()](#getFormat--) | Получает формат архива. |
| [getLength()](#getLength--) | Получает длину. |
| [getName()](#getName--) | Имя оригинального файла. |
| [save(File destination)](#save-java.io.File-) | Сохраняет snappy‑архив в указанный целевой файл. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Сохраняет snappy‑архив в указанный поток. |
| [save(String destinationFileName)](#save-java.lang.String-) | Сохраняет snappy‑архив в указанный целевой файл. |
| [setSource(File file)](#setSource-java.io.File-) | Устанавливает содержимое, которое будет сжато в архиве. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Устанавливает содержимое, которое будет сжато в архиве. |
| [setSource(String sourcePath)](#setSource-java.lang.String-) | Устанавливает содержимое, которое будет сжато в архиве. |
### SnappyArchive() {#SnappyArchive--}
```
public SnappyArchive()
```


Инициализирует новый экземпляр класса [SnappyArchive](../../com.aspose.zip/snappyarchive), подготовленный для сжатия.

Следующий пример показывает, как сжать файл.

```

``````

try (SnappyArchive archive = new SnappyArchive()) {
archive.setSource("data.bin");
archive.save("archive.snappy");
}
 
```



### SnappyArchive(InputStream source) {#SnappyArchive-java.io.InputStream-}
```
public SnappyArchive(InputStream source)
```


Initializes a new instance of the [SnappyArchive](../../com.aspose.zip/snappyarchive) class prepared for decompressing.

This constructor does not decompress. See [extract(java.io.OutputStream)](../../com.aspose.zip/snappyarchive\#extract-java.io.OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | The source of the archive. |

### SnappyArchive(String path) {#SnappyArchive-java.lang.String-}
```
public SnappyArchive(String path)
```


Initializes a new instance of the [SnappyArchive](../../com.aspose.zip/snappyarchive) class prepared for decompressing.

```

``````

      try (FileInputStream sourceSnappyFile = new FileInputStream("sourceFileName")) {
          try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
              try (SnappyArchive archive = new SnappyArchive(sourceSnappyFile)) {
                  archive.extract(extractedFile);
              }
          }
      } catch (IOException ex) {
      }
 
```

Этот конструктор не выполняет распаковку. См. метод [extract(java.io.OutputStream)](../../com.aspose.zip/snappyarchive\#extract-java.io.OutputStream-) для распаковки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| path | java.lang.String | путь к источнику архива |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Извлекает snappy‑архив в файл.

```

``````

try (FileInputStream snappyFile = new FileInputStream("sourceFileName")) {
try (SnappyArchive archive = new SnappyArchive(snappyFile)) {
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


Extracts snappy archive to a stream.

```

``````

     try (FileInputStream sourceSnappyFile = new FileInputStream("sourceFileName")) {
         try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
             try (SnappyArchive archive = new SnappyArchive(sourceSnappyFile)) {
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


Извлекает snappy‑архив в файл по пути.

```

``````

try (FileInputStream snappyFile = new FileInputStream("sourceFileName")) {
try (SnappyArchive archive = new SnappyArchive(snappyFile)) {
archive.extract("extracted.bin");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the file which will store decompressed data |

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

If the directory does not exist, it will be created |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the snappy archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the snappy archive
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


Gets length.

**Returns:**
java.lang.Long - length.
### getName() {#getName--}
```
public final String getName()
```


The name of original file.

**Returns:**
java.lang.String - the name of the original file
### save(File destination) {#save-java.io.File-}
```
public final void save(File destination)
```


Saves snappy archive to the destination file provided.

```

``````

     try (SnappyArchive archive = new SnappyArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(new File("archive.snappy"));
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| назначение | java.io.File | файл, который будет открыт как поток назначения |

### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Сохраняет snappy‑архив в указанный поток.

```

``````

try (FileOutputStream snappyFile = new FileOutputStream("archive.snappy")) {
try (SnappyArchive archive = new SnappyArchive()) {
archive.setSource("data.bin");
archive.save(snappyFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | the destination stream |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves snappy archive to the destination file provided.

```

``````

     try (SnappyArchive archive = new SnappyArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("result.snappy");
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| destinationFileName | java.lang.String | путь к создаваемому архиву. Если указанный файл уже существует, он будет перезаписан |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Устанавливает содержимое, которое будет сжато в архиве.

```

``````

try (SnappyArchive archive = new SnappyArchive()) {
archive.setSource(new File("data.bin"));
archive.save("archive.snappy");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | the file which will be opened as an input stream |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Sets the content to be compressed within the archive.

```

``````

     try (SnappyArchive archive = new SnappyArchive()) {
         archive.setSource(new ByteArrayInputStream(new byte[] {
                 0x00,
                 (byte) 0xFF
         }));
         archive.save("archive.snappy");
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| source | java.io.InputStream | входной поток для архива |

### setSource(String sourcePath) {#setSource-java.lang.String-}
```
public final void setSource(String sourcePath)
```


Устанавливает содержимое, которое будет сжато в архиве.

```

``````

try (SnappyArchive archive = new SnappyArchive()) {
archive.setSource("data.bin");
archive.save("archive.snappy");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourcePath | java.lang.String | the path to the file which will be opened as an input stream |

