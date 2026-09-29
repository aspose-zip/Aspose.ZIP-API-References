---
title: "UueArchive"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Этот класс представляет uuencoded файл."
type: docs
weight: 128
url: /ru/java/com.aspose.zip/uuearchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class UueArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

Этот класс представляет uuencoded файл.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [UueArchive()](#UueArchive--) | Инициализирует новый экземпляр класса [UueArchive](../../com.aspose.zip/uuearchive), подготовленного для кодирования. |
| [UueArchive(InputStream sourceStream)](#UueArchive-java.io.InputStream-) | Инициализирует новый экземпляр класса [UueArchive](../../com.aspose.zip/uuearchive), подготовленного для декодирования. |
| [UueArchive(String path)](#UueArchive-java.lang.String-) | Инициализирует новый экземпляр класса [UueArchive](../../com.aspose.zip/uuearchive). |
## Методы

| Метод | Описание |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Извлекает архив в указанный поток. |
| [extract(String path)](#extract-java.lang.String-) | Извлекает архив в файл по указанному пути. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Извлекает содержимое архива в указанную директорию. |
| [getFileEntries()](#getFileEntries--) | Получает элементы типа [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), составляющие uue‑архив. |
| [getFormat()](#getFormat--) | Получает формат архива. |
| [getLength()](#getLength--) | Получает длину. |
| [getName()](#getName--) | Имя оригинального файла. |
| [open()](#open--) | Открывает архив для декодирования и предоставляет поток с содержимым архива. |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | Сохраняет архив в предоставленный поток. |
| [save(OutputStream outputStream, UueSaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.UueSaveOptions-) | Сохраняет архив в предоставленный поток. |
| [save(String destinationFileName)](#save-java.lang.String-) | Сохраняет архив в указанный файл назначения. |
| [save(String destinationFileName, UueSaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.UueSaveOptions-) | Сохраняет архив в указанный файл назначения. |
| [setSource(File file)](#setSource-java.io.File-) | Устанавливает содержимое, которое будет сжато в архиве. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Устанавливает содержимое, которое будет закодировано в архиве. |
| [setSource(String path)](#setSource-java.lang.String-) | Устанавливает содержимое, которое будет закодировано в архиве. |
### UueArchive() {#UueArchive--}
```
public UueArchive()
```


Инициализирует новый экземпляр класса [UueArchive](../../com.aspose.zip/uuearchive), подготовленного для кодирования.

Следующий пример показывает, как выполнить uuencode файла.

```

``````

try (UueArchive archive = new UueArchive()) {
archive.setSource("data.bin");
archive.save("archive.uue");
}
 
```



### UueArchive(InputStream sourceStream) {#UueArchive-java.io.InputStream-}
```
public UueArchive(InputStream sourceStream)
```


Initializes a new instance of the [UueArchive](../../com.aspose.zip/uuearchive) class prepared for decoding.

Open an archive from a stream and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (UueArchive archive = new UueArchive(new FileInputStream("archive.001"))) {
         InputStream decompressed = archive.open();
         byte[] b = new byte[8192];
         int bytesRead;
         while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
     }
 
```

Этот конструктор не декодирует. См. метод [open()](../../com.aspose.zip/uuearchive\#open--) для распаковки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceStream | java.io.InputStream | источник архива |

### UueArchive(String path) {#UueArchive-java.lang.String-}
```
public UueArchive(String path)
```


Инициализирует новый экземпляр класса [UueArchive](../../com.aspose.zip/uuearchive).

Откройте архив из файла по пути и декодируйте его в `MemoryStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (UueArchive archive = new UueArchive(new FileInputStream("archive.uue"))) {
InputStream decompressed = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
}
 
```

This constructor does not decode. See [open()](../../com.aspose.zip/uuearchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

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

     try (UueArchive archive = new UueArchive("archive.uue")) {
         archive.extract(httpResponseStream);
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| назначение | java.io.OutputStream | поток назначения |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Извлекает архив в файл по указанному пути.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| path | java.lang.String | путь к целевому файлу. Если файл уже существует, он будет перезаписан. |

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


Получает элементы типа [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), составляющие uue‑архив.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; — элементы типа [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), составляющие uue‑архив
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
### open() {#open--}
```
public final InputStream open()
```


Открывает архив для декодирования и предоставляет поток с содержимым архива.

Использование:

```

``````

try (InputStream decompressed = archive.open()) {
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
fileStream.write(buffer, 0, bytesRead);
}
} catch (IOException ex) {
}
 
```

Read from the stream to get the original content of the file. See examples section.

**Returns:**
java.io.InputStream - the stream that represents the contents of the archive
### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


Saves archive to the stream provided.

Write compressed data to http response stream.

```

``````

     try (UueArchive archive = new UueArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(outputStream);
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| outputStream | java.io.OutputStream | поток назначения |

### save(OutputStream outputStream, UueSaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.UueSaveOptions-}
```
public final void save(OutputStream outputStream, UueSaveOptions saveOptions)
```


Сохраняет архив в предоставленный поток.

Запишите сжатые данные в поток ответа http.

```

``````

try (UueArchive archive = new UueArchive()) {
archive.setSource(new File("data.bin"));
archive.save(outputStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outputStream | java.io.OutputStream | destination stream |
| saveOptions | [UueSaveOptions](../../com.aspose.zip/uuesaveoptions) | options for the archive saving |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves the archive to the destination file provided.

Write encoded data to file.

```

``````

     try (UueArchive archive = new UueArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("data.uue");
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| destinationFileName | java.lang.String | путь к создаваемому архиву. Если указанный файл уже существует, он будет перезаписан |

### save(String destinationFileName, UueSaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.UueSaveOptions-}
```
public final void save(String destinationFileName, UueSaveOptions saveOptions)
```


Сохраняет архив в указанный файл назначения.

Записать закодированные данные в файл.

```

``````

try (UueArchive archive = new UueArchive()) {
archive.setSource(new File("data.bin"));
archive.save("data.uue");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| saveOptions | [UueSaveOptions](../../com.aspose.zip/uuesaveoptions) | options for the archive saving |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Sets the content to be compressed within the archive.

```

``````

     try (UueArchive archive = new UueArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.uue");
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| file | java.io.File | ссылка на файл, который будет сжат |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Устанавливает содержимое, которое будет закодировано в архиве.

```

``````

try (UueArchive archive = new UueArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] {
0x00,
(byte) 0xFF
}));
archive.save("archive.uue");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | the input stream for the archive |

### setSource(String path) {#setSource-java.lang.String-}
```
public final void setSource(String path)
```


Sets the content to be encoded within the archive.

```

``````

     try (UueArchive archive = new UueArchive()) {
         archive.setSource("data.bin");
         archive.save("archive.uue");
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| path | java.lang.String | путь к файлу, который будет кодироваться |

