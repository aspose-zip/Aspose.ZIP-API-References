---
title: "XarArchive"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Этот класс представляет файл архива xar."
type: docs
weight: 136
url: /ru/java/com.aspose.zip/xararchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class XarArchive implements IArchive, AutoCloseable
```

Этот класс представляет файл архива xar.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [XarArchive()](#XarArchive--) | Инициализирует новый экземпляр класса [XarArchive](../../com.aspose.zip/xararchive). |
| [XarArchive(XarCompressionSettings defaultCompressionSettings)](#XarArchive-com.aspose.zip.XarCompressionSettings-) | Инициализирует новый экземпляр класса [XarArchive](../../com.aspose.zip/xararchive). |
| [XarArchive(InputStream sourceStream)](#XarArchive-java.io.InputStream-) | Инициализирует новый экземпляр класса [XarArchive](../../com.aspose.zip/xararchive) и формирует список записей, которые могут быть извлечены из архива. |
| [XarArchive(InputStream sourceStream, XarLoadOptions loadOptions)](#XarArchive-java.io.InputStream-com.aspose.zip.XarLoadOptions-) | Инициализирует новый экземпляр класса [XarArchive](../../com.aspose.zip/xararchive) и формирует список записей, которые могут быть извлечены из архива. |
| [XarArchive(String path)](#XarArchive-java.lang.String-) | Инициализирует новый экземпляр класса [XarArchive](../../com.aspose.zip/xararchive) и формирует список записей, которые могут быть извлечены из архива. |
| [XarArchive(String path, XarLoadOptions loadOptions)](#XarArchive-java.lang.String-com.aspose.zip.XarLoadOptions-) | Инициализирует новый экземпляр класса [XarArchive](../../com.aspose.zip/xararchive) и формирует список записей, которые могут быть извлечены из архива. |
## Методы

| Метод | Описание |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога. |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога. |
| [createEntries(File directory, boolean includeRootDirectory, XarCompressionSettings compressionSettings)](#createEntries-java.io.File-boolean-com.aspose.zip.XarCompressionSettings-) | Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога. |
| [createEntries(String sourceDirectory)](#createEntries-java.lang.String-) | Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога. |
| [createEntries(String sourceDirectory, boolean includeRootDirectory)](#createEntries-java.lang.String-boolean-) | Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога. |
| [createEntries(String sourceDirectory, boolean includeRootDirectory, XarCompressionSettings compressionSettings)](#createEntries-java.lang.String-boolean-com.aspose.zip.XarCompressionSettings-) | Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога. |
| [createEntry(String name, File file)](#createEntry-java.lang.String-java.io.File-) | Создайте одну запись в архиве. |
| [createEntry(String name, File file, boolean openImmediately)](#createEntry-java.lang.String-java.io.File-boolean-) | Создайте одну запись в архиве. |
| [createEntry(String name, File file, boolean openImmediately, XarCompressionSettings compressionSettings)](#createEntry-java.lang.String-java.io.File-boolean-com.aspose.zip.XarCompressionSettings-) | Создайте одну запись в архиве. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | Создайте одну запись в архиве. |
| [createEntry(String name, InputStream source, XarCompressionSettings compressionSettings)](#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.XarCompressionSettings-) | Создайте одну запись в архиве. |
| [createEntry(String name, String sourcePath)](#createEntry-java.lang.String-java.lang.String-) | Создайте одну запись в архиве. |
| [createEntry(String name, String sourcePath, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | Создайте одну запись в архиве. |
| [createEntry(String name, String sourcePath, boolean openImmediately, XarCompressionSettings compressionSettings)](#createEntry-java.lang.String-java.lang.String-boolean-com.aspose.zip.XarCompressionSettings-) | Создайте одну запись в архиве. |
| [deleteEntry(XarEntry entry)](#deleteEntry-com.aspose.zip.XarEntry-) | Удаляет первое вхождение конкретной записи из списка записей. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Извлекает все файлы из архива в указанный каталог. |
| [getEntries()](#getEntries--) | Получает элементы типа [XarEntry](../../com.aspose.zip/xarentry), составляющие архив. |
| [getFileEntries()](#getFileEntries--) | Получает элементы типа [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), составляющие xar-архив. |
| [getFormat()](#getFormat--) | Получает формат архива. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Сохраняет архив в предоставленный поток. |
| [save(OutputStream output, XarSaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.XarSaveOptions-) | Сохраняет архив в предоставленный поток. |
| [save(String destinationFileName)](#save-java.lang.String-) | Сохраняет архив в указанный файл назначения. |
| [save(String destinationFileName, XarSaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.XarSaveOptions-) | Сохраняет архив в указанный файл назначения. |
### XarArchive() {#XarArchive--}
```
public XarArchive()
```


Инициализирует новый экземпляр класса [XarArchive](../../com.aspose.zip/xararchive).

Следующий пример показывает, как сжать файл.

```

``````

try (XarArchive archive = new XarArchive()) {
archive.createEntry("first.bin", "data.bin");
archive.save("archive.xar");
}
 
```



### XarArchive(XarCompressionSettings defaultCompressionSettings) {#XarArchive-com.aspose.zip.XarCompressionSettings-}
```
public XarArchive(XarCompressionSettings defaultCompressionSettings)
```


Initializes a new instance of the [XarArchive](../../com.aspose.zip/xararchive) class.

The following example shows how to compress a file.

```

``````

     try (XarArchive archive = new XarArchive()) {
         archive.createEntry("first.bin", "data.bin");
         archive.save("archive.xar");
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| defaultCompressionSettings | [XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings) | настройки сжатия по умолчанию, применяемые ко всем записям архива |

### XarArchive(InputStream sourceStream) {#XarArchive-java.io.InputStream-}
```
public XarArchive(InputStream sourceStream)
```


Инициализирует новый экземпляр класса [XarArchive](../../com.aspose.zip/xararchive) и формирует список записей, которые могут быть извлечены из архива.

В следующем примере показано, как извлечь все записи в каталог.

```

``````

try (XarArchive archive = new XarArchive(new FileInputStream("archive.xar"))) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry. See [XarFileEntry.open()](../../com.aspose.zip/xarfileentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |

### XarArchive(InputStream sourceStream, XarLoadOptions loadOptions) {#XarArchive-java.io.InputStream-com.aspose.zip.XarLoadOptions-}
```
public XarArchive(InputStream sourceStream, XarLoadOptions loadOptions)
```


Initializes a new instance of the [XarArchive](../../com.aspose.zip/xararchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (XarArchive archive = new XarArchive(new FileInputStream("archive.xar"))) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

Этот конструктор не распаковывает ни одну запись. См. метод [XarFileEntry.open()](../../com.aspose.zip/xarfileentry\#open--) для распаковки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceStream | java.io.InputStream | источник архива |
| loadOptions | [XarLoadOptions](../../com.aspose.zip/xarloadoptions) | параметры загрузки архива |

### XarArchive(String path) {#XarArchive-java.lang.String-}
```
public XarArchive(String path)
```


Инициализирует новый экземпляр класса [XarArchive](../../com.aspose.zip/xararchive) и формирует список записей, которые могут быть извлечены из архива.

В следующем примере показано, как извлечь все записи в каталог.

```

``````

try (XarArchive archive = new XarArchive(\"archive.xar\")) {
archive.extractToDirectory("C:\\extracted");
}
 
```

This constructor does not unpack any entry. See [XarFileEntry.open()](../../com.aspose.zip/xarfileentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### XarArchive(String path, XarLoadOptions loadOptions) {#XarArchive-java.lang.String-com.aspose.zip.XarLoadOptions-}
```
public XarArchive(String path, XarLoadOptions loadOptions)
```


Initializes a new instance of the [XarArchive](../../com.aspose.zip/xararchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (XarArchive archive = new XarArchive("archive.xar")) {
         archive.extractToDirectory("C:\\extracted");
     }
 
```

Этот конструктор не распаковывает ни одну запись. См. метод [XarFileEntry.open()](../../com.aspose.zip/xarfileentry\#open--) для распаковки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| path | java.lang.String | путь к файлу архива |
| loadOptions | [XarLoadOptions](../../com.aspose.zip/xarloadoptions) | параметры загрузки архива |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final XarArchive createEntries(File directory)
```


Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога.

```

``````

try (FileOutputStream xarFile = new FileOutputStream("archive.xar")) {
try (XarArchive archive = new XarArchive()) {
archive.createEntries(new java.io.File("C:\\folder"), false);
archive.save(xarFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | directory to compress |

**Returns:**
[XarArchive](../../com.aspose.zip/xararchive) - Xar entry instance
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final XarArchive createEntries(File directory, boolean includeRootDirectory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream xarFile = new FileOutputStream("archive.xar")) {
         try (XarArchive archive = new XarArchive()) {
             archive.createEntries(new java.io.File("C:\\folder"), false);
             archive.save(xarFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| directory | java.io.File | директория для сжатия |
| includeRootDirectory | boolean | указывает, следует ли включать корневой каталог сам по себе или нет |

**Returns:**
[XarArchive](../../com.aspose.zip/xararchive) - Xar entry instance
### createEntries(File directory, boolean includeRootDirectory, XarCompressionSettings compressionSettings) {#createEntries-java.io.File-boolean-com.aspose.zip.XarCompressionSettings-}
```
public final XarArchive createEntries(File directory, boolean includeRootDirectory, XarCompressionSettings compressionSettings)
```


Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога.

```

``````

try (FileOutputStream xarFile = new FileOutputStream("archive.xar")) {
try (XarArchive archive = new XarArchive()) {
archive.createEntries(new java.io.File("C:\\folder"), false);
archive.save(xarFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |
| compressionSettings | [XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings) | the compression settings used for added [XarEntry](../../com.aspose.zip/xarentry) items |

**Returns:**
[XarArchive](../../com.aspose.zip/xararchive) - Xar entry instance
### createEntries(String sourceDirectory) {#createEntries-java.lang.String-}
```
public final XarArchive createEntries(String sourceDirectory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream xarFile = new FileOutputStream("archive.xar")) {
         try (XarArchive archive = new XarArchive()) {
             archive.createEntries("C:\\folder", false);
             archive.save(xarFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceDirectory | java.lang.String | директория для сжатия |

**Returns:**
[XarArchive](../../com.aspose.zip/xararchive) - Xar entry instance
### createEntries(String sourceDirectory, boolean includeRootDirectory) {#createEntries-java.lang.String-boolean-}
```
public final XarArchive createEntries(String sourceDirectory, boolean includeRootDirectory)
```


Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога.

```

``````

try (FileOutputStream xarFile = new FileOutputStream("archive.xar")) {
try (XarArchive archive = new XarArchive()) {
archive.createEntries("C:\\folder", false);
archive.save(xarFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[XarArchive](../../com.aspose.zip/xararchive) - Xar entry instance
### createEntries(String sourceDirectory, boolean includeRootDirectory, XarCompressionSettings compressionSettings) {#createEntries-java.lang.String-boolean-com.aspose.zip.XarCompressionSettings-}
```
public final XarArchive createEntries(String sourceDirectory, boolean includeRootDirectory, XarCompressionSettings compressionSettings)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream xarFile = new FileOutputStream("archive.xar")) {
         try (XarArchive archive = new XarArchive()) {
             archive.createEntries("C:\\folder", false);
             archive.save(xarFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceDirectory | java.lang.String | директория для сжатия |
| includeRootDirectory | boolean | указывает, следует ли включать корневой каталог сам по себе или нет |
| compressionSettings | [XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings) | Настройки сжатия, используемые для добавленных элементов [XarEntry](../../com.aspose.zip/xarentry) |

**Returns:**
[XarArchive](../../com.aspose.zip/xararchive) - Xar entry instance
### createEntry(String name, File file) {#createEntry-java.lang.String-java.io.File-}
```
public final XarEntry createEntry(String name, File file)
```


Создайте одну запись в архиве.

```

``````

java.io.File file = new java.io.File("data.bin");
try (XarArchive archive = new XarArchive()) {
archive.createEntry("test.bin", file);
archive.save("archive.xar");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file or folder to be compressed |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### createEntry(String name, File file, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final XarEntry createEntry(String name, File file, boolean openImmediately)
```


Create a single entry within the archive.

```

``````

     java.io.File file = new java.io.File("data.bin");
     try (XarArchive archive = new XarArchive()) {
         archive.createEntry("test.bin", file);
         archive.save("archive.xar");
     }
 
```

Если файл открывается сразу с параметром `openImmediately`, он блокируется до тех пор, пока архив не будет освобождён

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| имя | java.lang.String | имя элемента |
| file | java.io.File | метаданные файла или папки, которые будут сжаты |
| openImmediately | boolean | true, если открыть файл сразу, иначе открыть файл при сохранении архива. |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### createEntry(String name, File file, boolean openImmediately, XarCompressionSettings compressionSettings) {#createEntry-java.lang.String-java.io.File-boolean-com.aspose.zip.XarCompressionSettings-}
```
public final XarEntry createEntry(String name, File file, boolean openImmediately, XarCompressionSettings compressionSettings)
```


Создайте одну запись в архиве.

```

``````

java.io.File file = new java.io.File("data.bin");
try (XarArchive archive = new XarArchive()) {
archive.createEntry("test.bin", file);
archive.save("archive.xar");
}
 
```

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is disposed

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file or folder to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving. |
| compressionSettings | [XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings) | the compression settings used for added [XarEntry](../../com.aspose.zip/xarentry) item |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final XarEntry createEntry(String name, InputStream source)
```


Create a single entry within the archive.

```

``````

     try (XarArchive archive = new XarArchive()) {
         archive.createEntry("data.bin", new FileInputStream("data.bin"));
         archive.save("archive.xar");
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| имя | java.lang.String | имя элемента |
| source | java.io.InputStream | входной поток для записи |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### createEntry(String name, InputStream source, XarCompressionSettings compressionSettings) {#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.XarCompressionSettings-}
```
public final XarEntry createEntry(String name, InputStream source, XarCompressionSettings compressionSettings)
```


Создайте одну запись в архиве.

```

``````

try (XarArchive archive = new XarArchive()) {
archive.createEntry("data.bin", new FileInputStream("data.bin"));
archive.save("archive.xar");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| source | java.io.InputStream | the input stream for the entry |
| compressionSettings | [XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings) | the compression settings used for added [XarEntry](../../com.aspose.zip/xarentry) item |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### createEntry(String name, String sourcePath) {#createEntry-java.lang.String-java.lang.String-}
```
public final XarEntry createEntry(String name, String sourcePath)
```


Create a single entry within the archive.

```

``````

     try (XarArchive archive = new XarArchive()) {
         archive.createEntry("first.bin", "data.bin");
         archive.save("archive.xar");
     }
 
```

Имя записи задаётся исключительно параметром `name`. Имя файла, указанное в параметре `sourcePath`, не влияет на имя записи.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| имя | java.lang.String | имя элемента |
| sourcePath | java.lang.String | Путь к файлу для сжатия |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### createEntry(String name, String sourcePath, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final XarEntry createEntry(String name, String sourcePath, boolean openImmediately)
```


Создайте одну запись в архиве.

```

``````

try (XarArchive archive = new XarArchive()) {
archive.createEntry("first.bin", "data.bin");
archive.save("archive.xar");
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `sourcePath` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is disposed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| sourcePath | java.lang.String | the path to the file to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### createEntry(String name, String sourcePath, boolean openImmediately, XarCompressionSettings compressionSettings) {#createEntry-java.lang.String-java.lang.String-boolean-com.aspose.zip.XarCompressionSettings-}
```
public final XarEntry createEntry(String name, String sourcePath, boolean openImmediately, XarCompressionSettings compressionSettings)
```


Create a single entry within the archive.

```

``````

     try (XarArchive archive = new XarArchive()) {
         archive.createEntry("first.bin", "data.bin");
         archive.save("archive.xar");
     }
 
```

Имя записи задаётся исключительно параметром `name`. Имя файла, указанное в параметре `sourcePath`, не влияет на имя записи.

Если файл открывается сразу с параметром `openImmediately`, он блокируется до тех пор, пока архив не будет освобождён.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| имя | java.lang.String | имя элемента |
| sourcePath | java.lang.String | Путь к файлу для сжатия |
| openImmediately | boolean | true, если открыть файл сразу, иначе открыть файл при сохранении архива |
| compressionSettings | [XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings) | Настройки сжатия, используемые для добавленного элемента [XarEntry](../../com.aspose.zip/xarentry) |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### deleteEntry(XarEntry entry) {#deleteEntry-com.aspose.zip.XarEntry-}
```
public final XarArchive deleteEntry(XarEntry entry)
```


Удаляет первое вхождение конкретной записи из списка записей.

Вот как можно удалить все записи, кроме последней:

```

``````

try (XarArchive archive = new XarArchive(\"archive.xar\")) {
while (archive.getEntries().size() > 1)
archive.deleteEntry(archive.getEntries().get(0));
archive.save("outputXarFile.xar");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| entry | [XarEntry](../../com.aspose.zip/xarentry) | the entry to remove from the entries list |

**Returns:**
[XarArchive](../../com.aspose.zip/xararchive) - Xar entry instance
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all the files in the archive to the directory provided.

```

``````

     try (XarArchive archive = new XarArchive("archive.xar")) {
         archive.extractToDirectory("C:\\extracted");
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | destinationDirectory | java.lang.String | путь к каталогу, в который будут помещены извлечённые файлы. |

Если каталог не существует, он будет создан |

### getEntries() {#getEntries--}
```
public final List<XarEntry> getEntries()
```


Получает элементы типа [XarEntry](../../com.aspose.zip/xarentry), составляющие архив.

**Returns:**
java.util.List&lt;com.aspose.zip.XarEntry&gt; - элементы типа [XarEntry](../../com.aspose.zip/xarentry), составляющие архив
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Получает элементы типа [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), составляющие xar-архив.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - элементы типа [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), составляющие xar‑архив
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Получает формат архива.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Сохраняет архив в предоставленный поток.

Для больших архивов используйте [save(String)](../../com.aspose.zip/xararchive\#save-String-), вместо сохранения в java.io.FileOutputStream.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| output | java.io.OutputStream | поток назначения |

### save(OutputStream output, XarSaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.XarSaveOptions-}
```
public final void save(OutputStream output, XarSaveOptions saveOptions)
```


Сохраняет архив в предоставленный поток.

Для больших архивов используйте [save(String)](../../com.aspose.zip/xararchive\#save-String-), вместо сохранения в java.io.FileOutputStream.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| output | java.io.OutputStream | поток назначения |
| saveOptions | [XarSaveOptions](../../com.aspose.zip/xarsaveoptions) | Опции для сохранения xar‑архива |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Сохраняет архив в указанный файл назначения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| destinationFileName | java.lang.String | путь к создаваемому архиву. Если указанный файл уже существует, он будет перезаписан |

### save(String destinationFileName, XarSaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.XarSaveOptions-}
```
public final void save(String destinationFileName, XarSaveOptions saveOptions)
```


Сохраняет архив в указанный файл назначения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| destinationFileName | java.lang.String | путь к создаваемому архиву. Если указанный файл уже существует, он будет перезаписан |
| saveOptions | [XarSaveOptions](../../com.aspose.zip/xarsaveoptions) | Опции для сохранения xar‑архива |

