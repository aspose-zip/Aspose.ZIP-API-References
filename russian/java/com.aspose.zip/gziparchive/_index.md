---
title: "GzipArchive"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Этот класс представляет файл gzip‑архива."
type: docs
weight: 69
url: /ru/java/com.aspose.zip/gziparchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class GzipArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

Этот класс представляет файл gzip-архива. Используйте его для создания или извлечения gzip-архивов.

Алгоритм сжатия Gzip основан на алгоритме DEFLATE, который представляет собой комбинацию LZ77 и кодирования Хаффмана.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [GzipArchive()](#GzipArchive--) | Инициализирует новый экземпляр класса [GzipArchive](../../com.aspose.zip/gziparchive), подготовленный для сжатия. |
| [GzipArchive(InputStream sourceStream)](#GzipArchive-java.io.InputStream-) | Инициализирует новый экземпляр класса [GzipArchive](../../com.aspose.zip/gziparchive), подготовленный для распаковки. |
| [GzipArchive(InputStream sourceStream, boolean parseHeader)](#GzipArchive-java.io.InputStream-boolean-) | Инициализирует новый экземпляр класса [GzipArchive](../../com.aspose.zip/gziparchive), подготовленный для распаковки. |
| [GzipArchive(InputStream sourceStream, GzipLoadOptions options)](#GzipArchive-java.io.InputStream-com.aspose.zip.GzipLoadOptions-) | Инициализирует новый экземпляр класса [GzipArchive](../../com.aspose.zip/gziparchive), подготовленный для распаковки. |
| [GzipArchive(String path, GzipLoadOptions options)](#GzipArchive-java.lang.String-com.aspose.zip.GzipLoadOptions-) | Инициализирует новый экземпляр класса [GzipArchive](../../com.aspose.zip/gziparchive), подготовленный для распаковки. |
| [GzipArchive(String path)](#GzipArchive-java.lang.String-) | Инициализирует новый экземпляр класса [GzipArchive](../../com.aspose.zip/gziparchive). |
| [GzipArchive(String path, boolean parseHeader)](#GzipArchive-java.lang.String-boolean-) | Инициализирует новый экземпляр класса [GzipArchive](../../com.aspose.zip/gziparchive). |
## Методы

| Метод | Описание |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Извлекает архив в указанный поток. |
| [extract(String path)](#extract-java.lang.String-) | Извлекает архив в файл по указанному пути. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Извлекает содержимое архива в указанную директорию. |
| [getFileEntries()](#getFileEntries--) | Получает элементы типа [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), составляющие gzip-архив. |
| [getFormat()](#getFormat--) | Получает формат архива. |
| [getLength()](#getLength--) | Получает размер оригинального файла. |
| [getName()](#getName--) | Имя оригинального файла. |
| [getUncompressedSize()](#getUncompressedSize--) | Получает размер оригинального файла. |
| [open()](#open--) | Открывает архив для извлечения и предоставляет поток с содержимым архива. |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | Сохраняет архив в предоставленный поток. |
| [save(String destinationFileName)](#save-java.lang.String-) | Сохраняет архив в указанный файл назначения. |
| [setSource(TarArchive tarArchive)](#setSource-com.aspose.zip.TarArchive-) | Устанавливает содержимое, которое будет сжато в архиве. |
| [setSource(File file)](#setSource-java.io.File-) | Устанавливает содержимое, которое будет сжато в архиве. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Устанавливает содержимое, которое будет сжато в архиве. |
| [setSource(String path)](#setSource-java.lang.String-) | Устанавливает содержимое, которое будет сжато в архиве. |
### GzipArchive() {#GzipArchive--}
```
public GzipArchive()
```


Инициализирует новый экземпляр класса [GzipArchive](../../com.aspose.zip/gziparchive), подготовленный для сжатия.

Следующий пример показывает, как сжать файл.

```

``````

try (GzipArchive archive = new GzipArchive())
{
archive.setSource("data.bin");
archive.save("archive.gz");
}
 
```



### GzipArchive(InputStream sourceStream) {#GzipArchive-java.io.InputStream-}
```
public GzipArchive(InputStream sourceStream)
```


Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class prepared for decompressing.

Open an archive from a stream and extract it to a `ByteArrayOutputStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (GzipArchive archive = new GzipArchive(Files.newInputStream(java.nio.file.Paths.get("archive.gz")))) {
         byte[] b = new byte[8192];
         int bytesRead;
         InputStream archiveStream = archive.open();
         while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

Этот конструктор не выполняет распаковку. См. метод [open()](../../com.aspose.zip/gziparchive\#open--) для распаковки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceStream | java.io.InputStream | Источник архива. |

### GzipArchive(InputStream sourceStream, boolean parseHeader) {#GzipArchive-java.io.InputStream-boolean-}
```
public GzipArchive(InputStream sourceStream, boolean parseHeader)
```


Инициализирует новый экземпляр класса [GzipArchive](../../com.aspose.zip/gziparchive), подготовленный для распаковки.

Откройте архив из потока и извлеките его в `ByteArrayOutputStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (GzipArchive archive = new GzipArchive(Files.newInputStream(java.nio.file.Paths.get("archive.gz")))) {
byte[] b = new byte[8192];
int bytesRead;
InputStream archiveStream = archive.open();
while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/gziparchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | The source of the archive. |
| parseHeader | boolean | Whether to parse stream header to figure out properties, including name. Makes sense for seekable stream only. |

### GzipArchive(InputStream sourceStream, GzipLoadOptions options) {#GzipArchive-java.io.InputStream-com.aspose.zip.GzipLoadOptions-}
```
public GzipArchive(InputStream sourceStream, GzipLoadOptions options)
```


Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class prepared for decompressing.

Open an archive from a stream and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     GzipLoadOptions options = new GzipLoadOptions();
     try (GzipArchive archive = new GzipArchive(new FileInputStream("archive.gz"), options)) {
         archive.extract(ms);
     } catch (IOException ex) {
     }
 
```

Этот конструктор не выполняет распаковку. См. метод [open()](../../com.aspose.zip/gziparchive\#open--) для распаковки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceStream | java.io.InputStream | Источник архива. |
| options | [GzipLoadOptions](../../com.aspose.zip/gziploadoptions) | Параметры загрузки архива. |

### GzipArchive(String path, GzipLoadOptions options) {#GzipArchive-java.lang.String-com.aspose.zip.GzipLoadOptions-}
```
public GzipArchive(String path, GzipLoadOptions options)
```


Инициализирует новый экземпляр класса [GzipArchive](../../com.aspose.zip/gziparchive), подготовленный для распаковки.

Откройте архив из файла по пути и извлеките его в `MemoryStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
GzipLoadOptions options = new GzipLoadOptions();
try (GzipArchive archive = new GzipArchive("archive.gz", options)) {
archive.extract(ms);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/gziparchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path to the archive file. |
| options | [GzipLoadOptions](../../com.aspose.zip/gziploadoptions) | Options to load the archive with. |

### GzipArchive(String path) {#GzipArchive-java.lang.String-}
```
public GzipArchive(String path)
```


Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class.

Open an archive from file by path and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (GzipArchive archive = new GzipArchive("archive.gz")) {
         byte[] b = new byte[8192];
         int bytesRead;
         InputStream archiveStream = archive.open();
         while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

Этот конструктор не выполняет распаковку. См. метод [open()](../../com.aspose.zip/gziparchive\#open--) для распаковки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| path | java.lang.String | Путь к файлу архива. |

### GzipArchive(String path, boolean parseHeader) {#GzipArchive-java.lang.String-boolean-}
```
public GzipArchive(String path, boolean parseHeader)
```


Инициализирует новый экземпляр класса [GzipArchive](../../com.aspose.zip/gziparchive).

Откройте архив из файла по пути и извлеките его в `MemoryStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (GzipArchive archive = new GzipArchive("archive.gz")) {
byte[] b = new byte[8192];
int bytesRead;
InputStream archiveStream = archive.open();
while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/gziparchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path to the archive file. |
| parseHeader | boolean | Whether to parse stream header to figure out properties, including name. Makes sense for seekable stream only. |

### close() {#close--}
```
public void close()
```




### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts the archive to the stream provided.

```

``````

     try (GzipArchive archive = new GzipArchive("archive.gz")) {
         archive.extract(httpResponseStream);
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| назначение | java.io.OutputStream | Поток назначения. Должен быть доступен для записи. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Извлекает архив в файл по указанному пути.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| path | java.lang.String | Путь к файлу назначения. Если файл уже существует, он будет перезаписан. |

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
|  | destinationDirectory | java.lang.String | Путь к каталогу, в который будут помещены извлечённые файлы. |

Если каталог не существует, он будет создан. |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Получает элементы типа [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), составляющие gzip-архив.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - элементы типа [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), составляющие gzip‑архив.
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


Получает размер оригинального файла.

Во время распаковки это свойство может содержать неверный размер. Если размер распакованного файла превышает 4 ГБ, это свойство даст неправильное значение из‑за 32‑битного ограничения в заголовке.

**Returns:**
java.lang.Long - размер оригинального файла
### getName() {#getName--}
```
public final String getName()
```


Имя оригинального файла.

**Returns:**
java.lang.String - имя оригинального файла
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Получает размер оригинального файла.

Во время распаковки это свойство может содержать неверный размер. Если размер распакованного файла превышает 4 ГБ, это свойство даст неправильное значение из‑за 32‑битного ограничения в заголовке.

**Returns:**
long - размер оригинального файла.
### open() {#open--}
```
public final InputStream open()
```


Открывает архив для извлечения и предоставляет поток с содержимым архива.

Извлекает архив и копирует извлечённое содержимое в файловый поток.

```

``````

try (GzipArchive archive = new GzipArchive("archive.gz")) {
try (FileOutputStream extracted = new FileOutputStream(\"data.bin\")) {
InputStream unpacked = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = unpacked.read(b, 0, b.length))) {
extracted.write(b, 0, bytesRead);
}
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

Read from the stream to get the original content of a file. See examples section.

**Returns:**
java.io.InputStream - The stream that represents the contents of the archive.
### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


Saves archive to the stream provided.

Writes compressed data to http response stream.

```

``````

     try (GzipArchive archive = new GzipArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(httpResponseStream);
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | outputStream | java.io.OutputStream | Поток назначения. |

`outputStream` должен быть доступен для записи. |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Сохраняет архив в указанный файл назначения.

```

``````

try (GzipArchive archive = new GzipArchive()) {
archive.setSource("data.bin");
archive.save("archive.gz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |

### setSource(TarArchive tarArchive) {#setSource-com.aspose.zip.TarArchive-}
```
public final void setSource(TarArchive tarArchive)
```


Sets the content to be compressed within the archive.

```

``````

     try (TarArchive tarArchive = new TarArchive()) {
         tarArchive.createEntry("first.bin", "data1.bin");
         tarArchive.createEntry("second.bin", "data2.bin");
         try (GzipArchive gzippedArchive = new GzipArchive()) {
             gzippedArchive.setSource(tarArchive);
             gzippedArchive.save("archive.tar.gz");
         }
     }
 
```

Используйте этот метод для создания объединённого tar.gz‑архива.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| tarArchive | [TarArchive](../../com.aspose.zip/tararchive) | Tar-архив для сжатия. |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Устанавливает содержимое, которое будет сжато в архиве.

```

``````

try (GzipArchive archive = new GzipArchive()) {
archive.setSource(new File("data.bin"));
archive.save("archive.gz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | The reference to a file to be compressed. |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Sets the content to be compressed within the archive.

```

``````

     try (GzipArchive archive = new GzipArchive()) {
         archive.setSource(new ByteArrayInputStream(new byte[] {
                 0x00,
                 (byte) 0xFF
         }));
         archive.save("archive.gz");
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| source | java.io.InputStream | Входной поток для архива. |

### setSource(String path) {#setSource-java.lang.String-}
```
public final void setSource(String path)
```


Устанавливает содержимое, которое будет сжато в архиве.

Откройте архив из файла по пути и извлеките его в `MemoryStream`

```

``````

try (GzipArchive archive = new GzipArchive()) {
archive.setSource("data.bin");
archive.save("archive.gz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | Path to file to be compressed. |

