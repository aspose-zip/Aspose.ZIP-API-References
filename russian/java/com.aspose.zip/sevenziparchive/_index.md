---
title: "SevenZipArchive"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Этот класс представляет файл 7z‑архива."
type: docs
weight: 104
url: /ru/java/com.aspose.zip/sevenziparchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class SevenZipArchive implements IArchive, AutoCloseable
```

Этот класс представляет файл архива 7z. Используйте его для создания и извлечения архивов 7z.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [SevenZipArchive()](#SevenZipArchive--) | Инициализирует новый экземпляр класса [SevenZipArchive](../../com.aspose.zip/sevenziparchive) с необязательными настройками для его записей. |
| [SevenZipArchive(SevenZipEntrySettings newEntrySettings)](#SevenZipArchive-com.aspose.zip.SevenZipEntrySettings-) | Инициализирует новый экземпляр класса [SevenZipArchive](../../com.aspose.zip/sevenziparchive) с необязательными настройками для его записей. |
| [SevenZipArchive(InputStream sourceStream)](#SevenZipArchive-java.io.InputStream-) | Инициализирует новый экземпляр класса [SevenZipArchive](../../com.aspose.zip/sevenziparchive) и формирует список записей, которые можно извлечь из архива. |
| [SevenZipArchive(InputStream sourceStream, String password)](#SevenZipArchive-java.io.InputStream-java.lang.String-) | Инициализирует новый экземпляр класса [SevenZipArchive](../../com.aspose.zip/sevenziparchive) и формирует список записей, которые можно извлечь из архива. |
| [SevenZipArchive(String path)](#SevenZipArchive-java.lang.String-) | Инициализирует новый экземпляр класса [SevenZipArchive](../../com.aspose.zip/sevenziparchive) и формирует список записей, которые можно извлечь из архива. |
| [SevenZipArchive(String path, String password)](#SevenZipArchive-java.lang.String-java.lang.String-) | Инициализирует новый экземпляр класса [SevenZipArchive](../../com.aspose.zip/sevenziparchive) и формирует список записей, которые можно извлечь из архива. |
| [SevenZipArchive(InputStream sourceStream, SevenZipLoadOptions options)](#SevenZipArchive-java.io.InputStream-com.aspose.zip.SevenZipLoadOptions-) | Инициализирует новый экземпляр класса [SevenZipArchive](../../com.aspose.zip/sevenziparchive) и формирует список записей, которые можно извлечь из архива. |
| [SevenZipArchive(String path, SevenZipLoadOptions options)](#SevenZipArchive-java.lang.String-com.aspose.zip.SevenZipLoadOptions-) | Инициализирует новый экземпляр класса [SevenZipArchive](../../com.aspose.zip/sevenziparchive) и формирует список записей, которые можно извлечь из архива. |
| [SevenZipArchive(String[] parts)](#SevenZipArchive-java.lang.String---) | Инициализирует новый экземпляр класса [SevenZipArchive](../../com.aspose.zip/sevenziparchive) из многотомного архива 7z и формирует список записей, которые можно извлечь из архива. |
| [SevenZipArchive(String[] parts, String password)](#SevenZipArchive-java.lang.String---java.lang.String-) | Инициализирует новый экземпляр класса [SevenZipArchive](../../com.aspose.zip/sevenziparchive) из многотомного архива 7z и формирует список записей, которые можно извлечь из архива. |
## Методы

| Метод | Описание |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога. |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога. |
| [createEntries(String sourceDirectory)](#createEntries-java.lang.String-) | Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога. |
| [createEntries(String sourceDirectory, boolean includeRootDirectory)](#createEntries-java.lang.String-boolean-) | Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога. |
| [createEntry(String name, File file)](#createEntry-java.lang.String-java.io.File-) | Создаёт одну запись внутри архива. |
| [createEntry(String name, File file, boolean openImmediately)](#createEntry-java.lang.String-java.io.File-boolean-) | Создаёт одну запись внутри архива. |
| [createEntry(String name, File file, boolean openImmediately, SevenZipEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.io.File-boolean-com.aspose.zip.SevenZipEntrySettings-) | Создаёт одну запись внутри архива. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | Создаёт одну запись внутри архива. |
| [createEntry(String name, InputStream source, SevenZipEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.SevenZipEntrySettings-) | Создаёт одну запись внутри архива. |
| [createEntry(String name, InputStream source, SevenZipEntrySettings newEntrySettings, File file)](#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.SevenZipEntrySettings-java.io.File-) | Создаёт одну запись внутри архива. |
| [createEntry(String name, String path)](#createEntry-java.lang.String-java.lang.String-) | Создаёт одну запись внутри архива. |
| [createEntry(String name, String path, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | Создаёт одну запись внутри архива. |
| [createEntry(String name, String path, boolean openImmediately, SevenZipEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.lang.String-boolean-com.aspose.zip.SevenZipEntrySettings-) | Создаёт одну запись внутри архива. |
| [createEntry(String name, Supplier&lt;InputStream&gt; streamProvider)](#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--) | Создайте одну запись в архиве. |
| [createEntry(String name, Supplier&lt;InputStream&gt; streamProvider, SevenZipEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--com.aspose.zip.SevenZipEntrySettings-) | Создайте одну запись в архиве. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Извлекает все файлы из архива в указанный каталог. |
| [extractToDirectory(String destinationDirectory, String password)](#extractToDirectory-java.lang.String-java.lang.String-) | Извлекает все файлы из архива в указанный каталог. |
| [getEntries()](#getEntries--) | Получает записи типа [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry), составляющие архив. |
| [getFileEntries()](#getFileEntries--) | Получает записи типа [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), составляющие архив 7z. |
| [getFormat()](#getFormat--) | Получает формат архива. |
| [getNewEntrySettings()](#getNewEntrySettings--) | Настройки сжатия и шифрования, используемые для недавно добавленных элементов [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry). |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Сохраняет архив 7z в предоставленный поток. |
| [save(OutputStream output, SevenZipArchiveSaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.SevenZipArchiveSaveOptions-) | Сохраняет архив 7z в предоставленный поток. |
| [save(String destinationFileName)](#save-java.lang.String-) | Сохраняет архив в указанный файл назначения. |
| [save(String destinationFileName, SevenZipArchiveSaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.SevenZipArchiveSaveOptions-) | Сохраняет архив в указанный файл назначения. |
| [saveSplit(String destinationDirectory, SplitSevenZipArchiveSaveOptions options)](#saveSplit-java.lang.String-com.aspose.zip.SplitSevenZipArchiveSaveOptions-) | Сохраняет многотомный архив в указанную целевую директорию. |
### SevenZipArchive() {#SevenZipArchive--}
```
public SevenZipArchive()
```


Инициализирует новый экземпляр класса [SevenZipArchive](../../com.aspose.zip/sevenziparchive) с необязательными настройками для его записей.

Следующий пример показывает, как сжать один файл с настройками по умолчанию: сжатие LZMA без шифрования.

```

``````

try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
try (SevenZipArchive archive = new SevenZipArchive()) {
archive.createEntry("data.bin", "file.dat");
archive.save(sevenZipFile);
}
} catch (IOException ex) {
}
 
```

LZMA compression without encryption would be used.

### SevenZipArchive(SevenZipEntrySettings newEntrySettings) {#SevenZipArchive-com.aspose.zip.SevenZipEntrySettings-}
```
public SevenZipArchive(SevenZipEntrySettings newEntrySettings)
```


Initializes a new instance of the [SevenZipArchive](../../com.aspose.zip/sevenziparchive) class with optional settings for its entries.

The following example shows how to compress a single file with default settings: LZMA compression without encryption.

```

``````

     try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
         try (SevenZipArchive archive = new SevenZipArchive()) {
             archive.createEntry("data.bin", "file.dat");
             archive.save(sevenZipFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| newEntrySettings | [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) | параметры сжатия и шифрования, используемые для вновь добавленных элементов [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry). Если не указано, будет использовано сжатие LZMA без шифрования |

### SevenZipArchive(InputStream sourceStream) {#SevenZipArchive-java.io.InputStream-}
```
public SevenZipArchive(InputStream sourceStream)
```


Инициализирует новый экземпляр класса [SevenZipArchive](../../com.aspose.zip/sevenziparchive) и формирует список записей, которые можно извлечь из архива.

```

``````

try (SevenZipArchive archive = new SevenZipArchive(new FileInputStream("archive.7z"))) {
archive.extractToDirectory("C:\\extracted");
} catch (FileNotFoundException ex) {
}
 
```

This constructor does not decompress any entry. See [extractToDirectory(String, String)](../../com.aspose.zip/sevenziparchive\#extractToDirectory-String--String-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |

### SevenZipArchive(InputStream sourceStream, String password) {#SevenZipArchive-java.io.InputStream-java.lang.String-}
```
public SevenZipArchive(InputStream sourceStream, String password)
```


Initializes a new instance of the [SevenZipArchive](../../com.aspose.zip/sevenziparchive) class and composes an entry list can be extracted from the archive.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive(new FileInputStream("archive.7z"))) {
         archive.extractToDirectory("C:\\extracted");
     } catch (FileNotFoundException ex) {
     }
 
```

Этот конструктор не распаковывает ни одну запись. См. метод [extractToDirectory(String, String)](../../com.aspose.zip/sevenziparchive\#extractToDirectory-String--String-) для распаковки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceStream | java.io.InputStream | источник архива |
| password | java.lang.String | необязательный пароль для расшифровки. Если имена файлов зашифрованы, он должен быть указан |

### SevenZipArchive(String path) {#SevenZipArchive-java.lang.String-}
```
public SevenZipArchive(String path)
```


Инициализирует новый экземпляр класса [SevenZipArchive](../../com.aspose.zip/sevenziparchive) и формирует список записей, которые можно извлечь из архива.

```

``````

try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
archive.extractToDirectory("C:\\extracted");
} catch (FileNotFoundException ex) {
}
 
```

This constructor does not decompress any entry. See [extractToDirectory(String, String)](../../com.aspose.zip/sevenziparchive\#extractToDirectory-String--String-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the fully qualified or the relative path to the archive file |

### SevenZipArchive(String path, String password) {#SevenZipArchive-java.lang.String-java.lang.String-}
```
public SevenZipArchive(String path, String password)
```


Initializes a new instance of the [SevenZipArchive](../../com.aspose.zip/sevenziparchive) class and composes an entry list can be extracted from the archive.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
         archive.extractToDirectory("C:\\extracted");
     } catch (FileNotFoundException ex) {
     }
 
```

Этот конструктор не распаковывает ни одну запись. См. метод [extractToDirectory(String, String)](../../com.aspose.zip/sevenziparchive\#extractToDirectory-String--String-) для распаковки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| path | java.lang.String | полный или относительный путь к файлу архива |
| password | java.lang.String | необязательный пароль для расшифровки. Если имена файлов зашифрованы, он должен быть указан |

### SevenZipArchive(InputStream sourceStream, SevenZipLoadOptions options) {#SevenZipArchive-java.io.InputStream-com.aspose.zip.SevenZipLoadOptions-}
```
public SevenZipArchive(InputStream sourceStream, SevenZipLoadOptions options)
```


Инициализирует новый экземпляр класса [SevenZipArchive](../../com.aspose.zip/sevenziparchive) и формирует список записей, которые можно извлечь из архива.

Извлеките зашифрованный архив. Разрешите выполнение до 60 секунд, после этого периода отмените.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
SevenZipLoadOptions options = new SevenZipLoadOptions();
options.setDecryptionPassword("Top$ecr3t");
options.setCancellationFlag(cf);
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
try (SevenZipArchive a = new SevenZipArchive(new FileInputStream("archive.7z"), options)) {
a.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | The source of the archive. |
| options | [SevenZipLoadOptions](../../com.aspose.zip/sevenziploadoptions) | Options to load existing archive with.

This constructor does not decompress any entry. See [extractToDirectory(String, String)](../../com.aspose.zip/sevenziparchive\#extractToDirectory-String--String-) method for decompressing. |

### SevenZipArchive(String path, SevenZipLoadOptions options) {#SevenZipArchive-java.lang.String-com.aspose.zip.SevenZipLoadOptions-}
```
public SevenZipArchive(String path, SevenZipLoadOptions options)
```


Initializes a new instance of the [SevenZipArchive](../../com.aspose.zip/sevenziparchive) class and composes an entry list can be extracted from the archive.

Extract an encrypted archive. Allow up to 60 seconds to proceed, cancel after that period.

```

``````

     try (CancellationFlag cf = new CancellationFlag()) {
         SevenZipLoadOptions options = new SevenZipLoadOptions();
         options.setDecryptionPassword("Top$ecr3t");
         options.setCancellationFlag(cf);
         cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
         try (SevenZipArchive a = new SevenZipArchive(new FileInputStream("archive.7z"), options)) {
             a.extractToDirectory("C:\\extracted");
         } catch (IOException ex) {
         }
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| path | java.lang.String | Полный или относительный путь к файлу архива. |
|  | options | [SevenZipLoadOptions](../../com.aspose.zip/sevenziploadoptions) | Параметры для загрузки существующего архива. |

Этот конструктор не распаковывает ни одну запись. См. метод [extractToDirectory(String, String)](../../com.aspose.zip/sevenziparchive\#extractToDirectory-String--String-) для распаковки. |

### SevenZipArchive(String[] parts) {#SevenZipArchive-java.lang.String---}
```
public SevenZipArchive(String[] parts)
```


Инициализирует новый экземпляр класса [SevenZipArchive](../../com.aspose.zip/sevenziparchive) из многотомного архива 7z и формирует список записей, которые можно извлечь из архива.

```

``````

try (SevenZipArchive archive = new SevenZipArchive(new String[] { "multi.7z.001", "multi.7z.002", "multi.7z.003" } )) {
archive.extractToDirectory("C:\\extracted");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| parts | java.lang.String[] | paths to each segment of multi-volume 7z archive respecting order |

### SevenZipArchive(String[] parts, String password) {#SevenZipArchive-java.lang.String---java.lang.String-}
```
public SevenZipArchive(String[] parts, String password)
```


Initializes a new instance of the [SevenZipArchive](../../com.aspose.zip/sevenziparchive) class from multi-volume 7z archive and composes an entry list can be extracted from the archive.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive(new String[] { "multi.7z.001", "multi.7z.002", "multi.7z.003" } )) {
         archive.extractToDirectory("C:\\extracted");
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| parts | java.lang.String[] | пути к каждому сегменту многотомного 7z архива в правильном порядке |
| password | java.lang.String | необязательный пароль для расшифровки. Если имена файлов зашифрованы, он должен быть указан |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final SevenZipArchive createEntries(File directory)
```


Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога.

```

``````

try (SevenZipArchive archive = new SevenZipArchive()) {
File folder = new File("C:\\folder");
archive.createEntries(folder);
archive.save("folder.7z");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | directory to compress |

**Returns:**
[SevenZipArchive](../../com.aspose.zip/sevenziparchive) - the archive with entries composed
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final SevenZipArchive createEntries(File directory, boolean includeRootDirectory)
```


Adds to the archive all files and directories recursively in the directory given.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive()) {
         File folder = new File("C:\\folder");
         archive.createEntries(folder);
         archive.save("folder.7z");
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| directory | java.io.File | директория для сжатия |
| includeRootDirectory | boolean | указывает, следует ли включать корневой каталог сам по себе или нет |

**Returns:**
[SevenZipArchive](../../com.aspose.zip/sevenziparchive) - the archive with entries composed
### createEntries(String sourceDirectory) {#createEntries-java.lang.String-}
```
public final SevenZipArchive createEntries(String sourceDirectory)
```


Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога.

Создайте 7z архив с сжатием LZMA.

```

``````

try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings()))) {
archive.createEntries("C:\\folder");
archive.save("folder.7z");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | directory to compress |

**Returns:**
[SevenZipArchive](../../com.aspose.zip/sevenziparchive) - the archive with entries composed
### createEntries(String sourceDirectory, boolean includeRootDirectory) {#createEntries-java.lang.String-boolean-}
```
public final SevenZipArchive createEntries(String sourceDirectory, boolean includeRootDirectory)
```


Adds to the archive all files and directories recursively in the directory given.

Compose 7z archive with LZMA compression.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings()))) {
         archive.createEntries("C:\\folder");
         archive.save("folder.7z");
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceDirectory | java.lang.String | директория для сжатия |
| includeRootDirectory | boolean | указывает, следует ли включать корневой каталог сам по себе или нет |

**Returns:**
[SevenZipArchive](../../com.aspose.zip/sevenziparchive) - the archive with entries composed
### createEntry(String name, File file) {#createEntry-java.lang.String-java.io.File-}
```
public final SevenZipArchiveEntry createEntry(String name, File file)
```


Создаёт одну запись внутри архива.

Создайте архив с записями, зашифрованными разными паролями.

```

``````

try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
File fi1 = new File("data1.bin");
File fi2 = new File("data2.bin");
File fi3 = new File("data3.bin");

try (SevenZipArchive archive = new SevenZipArchive()) {
archive.createEntry("entry1.bin", fi1, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test1")));
archive.createEntry("entry2.bin", fi2, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test2")));
archive.createEntry("entry3.bin", fi3, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test3")));
archive.save(sevenZipFile);
}
} catch (IOException ex) {
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `file` parameter does not affect the entry name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file to be compressed |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - Seven Zip entry instance
### createEntry(String name, File file, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final SevenZipArchiveEntry createEntry(String name, File file, boolean openImmediately)
```


Creates a single entry within the archive.

Compose archive with entries encrypted with different passwords each.

```

``````

     try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
         File fi1 = new File("data1.bin");
         File fi2 = new File("data2.bin");
         File fi3 = new File("data3.bin");

         try (SevenZipArchive archive = new SevenZipArchive()) {
             archive.createEntry("entry1.bin", fi1, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test1")));
             archive.createEntry("entry2.bin", fi2, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test2")));
             archive.createEntry("entry3.bin", fi3, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test3")));
             archive.save(sevenZipFile);
         }
     } catch (IOException ex) {
     }
 
```

Имя записи задаётся исключительно параметром `name`. Имя файла, переданное в параметре `file`, не влияет на имя записи.

Если файл открыт сразу с параметром `openImmediately`, он будет заблокирован до сохранения архива.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| имя | java.lang.String | имя элемента |
| file | java.io.File | метаданные файла, который будет сжат |
| openImmediately | boolean | true, если открыть файл сразу, иначе открыть файл при сохранении архива |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - Seven Zip entry instance
### createEntry(String name, File file, boolean openImmediately, SevenZipEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.io.File-boolean-com.aspose.zip.SevenZipEntrySettings-}
```
public final SevenZipArchiveEntry createEntry(String name, File file, boolean openImmediately, SevenZipEntrySettings newEntrySettings)
```


Создаёт одну запись внутри архива.

Создайте архив с записями, зашифрованными разными паролями.

```

``````

try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
File fi1 = new File("data1.bin");
File fi2 = new File("data2.bin");
File fi3 = new File("data3.bin");

try (SevenZipArchive archive = new SevenZipArchive()) {
archive.createEntry("entry1.bin", fi1, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test1")));
archive.createEntry("entry2.bin", fi2, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test2")));
archive.createEntry("entry3.bin", fi3, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test3")));
archive.save(sevenZipFile);
}
} catch (IOException ex) {
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `file` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is saved.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving |
| newEntrySettings | [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) | compression and encryption settings used for added [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) item. Individual compression settings is ignored in case of solid compression, see `SevenZipEntrySettings.Solid`([SevenZipEntrySettings.getSolid](../../com.aspose.zip/sevenzipentrysettings\#getSolid)/[SevenZipEntrySettings.setSolid](../../com.aspose.zip/sevenzipentrysettings\#setSolid)). |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - Seven Zip entry instance
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final SevenZipArchiveEntry createEntry(String name, InputStream source)
```


Creates a single entry within the archive.

Compose 7z archive with LZMA compression and encryption of all entries.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings(), new SevenZipAESEncryptionSettings("p@s$")))) {
         archive.createEntry("data.bin", new ByteArrayInputStream(new byte[] {0x00, (byte)0xFF} ));
         archive.save("archive.7z");
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| имя | java.lang.String | имя элемента |
| source | java.io.InputStream | входной поток для записи |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - Seven Zip entry instance
### createEntry(String name, InputStream source, SevenZipEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.SevenZipEntrySettings-}
```
public final SevenZipArchiveEntry createEntry(String name, InputStream source, SevenZipEntrySettings newEntrySettings)
```


Создаёт одну запись внутри архива.

Создайте 7z‑архив с LZMA‑сжатием и шифрованием всех записей.

```

``````

try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings(), new SevenZipAESEncryptionSettings("p@s$")))) {
archive.createEntry("data.bin", new ByteArrayInputStream(new byte[] {0x00, (byte)0xFF} ));
archive.save("archive.7z");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| source | java.io.InputStream | the input stream for the entry |
| newEntrySettings | [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) | compression and encryption settings used for added [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) item. Individual compression settings is ignored in case of solid compression, see `SevenZipEntrySettings.Solid`([SevenZipEntrySettings.getSolid](../../com.aspose.zip/sevenzipentrysettings\#getSolid)/[SevenZipEntrySettings.setSolid](../../com.aspose.zip/sevenzipentrysettings\#setSolid)). |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - Seven Zip entry instance
### createEntry(String name, InputStream source, SevenZipEntrySettings newEntrySettings, File file) {#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.SevenZipEntrySettings-java.io.File-}
```
public final SevenZipArchiveEntry createEntry(String name, InputStream source, SevenZipEntrySettings newEntrySettings, File file)
```


Creates a single entry within the archive.

Compose archive with LZMA compressed encrypted entry.

```

``````

     try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
         try (SevenZipArchive archive = new SevenZipArchive()) {
             archive.createEntry("entry1.bin", new ByteArrayInputStream(new byte[] {0x00, (byte)0xFF}), new SevenZipEntrySettings(new SevenZipLZMACompressionSettings(), new SevenZipAESEncryptionSettings("test1")), new File("data1.bin"));
             archive.save(sevenZipFile);
         }
     } catch (IOException ex) {
     }
 
```

Имя записи задаётся исключительно параметром `name`. Имя файла, переданное в параметре `file`, не влияет на имя записи.

`file` может указывать на каталог.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| имя | java.lang.String | имя элемента |
| source | java.io.InputStream | входной поток для записи |
| newEntrySettings | [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) | Настройки сжатия и шифрования, используемые для добавленного элемента [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry). Индивидуальные настройки сжатия игнорируются в случае сплошного сжатия, см. `SevenZipEntrySettings.Solid`([SevenZipEntrySettings.getSolid](../../com.aspose.zip/sevenzipentrysettings\#getSolid)/[SevenZipEntrySettings.setSolid](../../com.aspose.zip/sevenzipentrysettings\#setSolid)). |
| file | java.io.File | метаданные файла или папки, которые будут сжаты |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - Seven Zip entry instance
### createEntry(String name, String path) {#createEntry-java.lang.String-java.lang.String-}
```
public final SevenZipArchiveEntry createEntry(String name, String path)
```


Создаёт одну запись внутри архива.

```

``````

try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings()))) {
archive.createEntry("data.bin", "file.dat");
archive.save(sevenZipFile);
}
} catch (IOException ex) {
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `path` parameter does not affect the entry name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| path | java.lang.String | the fully qualified name of the new file, or the relative file name to be compressed |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - Seven Zip entry instance
### createEntry(String name, String path, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final SevenZipArchiveEntry createEntry(String name, String path, boolean openImmediately)
```


Creates a single entry within the archive.

```

``````

     try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
         try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings()))) {
             archive.createEntry("data.bin", "file.dat");
             archive.save(sevenZipFile);
         }
     } catch (IOException ex) {
     }
 
```

Имя элемента задаётся исключительно параметром `name`. Имя файла, переданное в параметре `path`, не влияет на имя элемента.

Если файл открыт сразу с параметром `openImmediately`, он будет заблокирован до сохранения архива.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| имя | java.lang.String | имя элемента |
| path | java.lang.String | полное квалифицированное имя нового файла, или относительное имя файла, который будет сжат |
| openImmediately | boolean | true, если открыть файл сразу, иначе открыть файл при сохранении архива |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - Seven Zip entry instance
### createEntry(String name, String path, boolean openImmediately, SevenZipEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.lang.String-boolean-com.aspose.zip.SevenZipEntrySettings-}
```
public final SevenZipArchiveEntry createEntry(String name, String path, boolean openImmediately, SevenZipEntrySettings newEntrySettings)
```


Создаёт одну запись внутри архива.

```

``````

try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings()))) {
archive.createEntry("data.bin", "file.dat");
archive.save(sevenZipFile);
}
} catch (IOException ex) {
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `path` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is saved.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| path | java.lang.String | the fully qualified name of the new file, or the relative file name to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving |
| newEntrySettings | [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) | compression and encryption settings used for added [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) item. Individual compression settings is ignored in case of solid compression, see `SevenZipEntrySettings.Solid`([SevenZipEntrySettings.getSolid](../../com.aspose.zip/sevenzipentrysettings\#getSolid)/[SevenZipEntrySettings.setSolid](../../com.aspose.zip/sevenzipentrysettings\#setSolid)). |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - Zip entry instance
### createEntry(String name, Supplier&lt;InputStream&gt; streamProvider) {#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--}
```
public final SevenZipArchiveEntry createEntry(String name, Supplier<InputStream> streamProvider)
```


Create a single entry within the archive.

Compose archive with LZMA2 compressed encrypted entry.

```

``````

 System.Func&lt;Stream&gt; provider = delegate(){ return new MemoryStream(new byte[]{0xFF, 0x00}); };
 using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
 {
     using (var archive = new SevenZipArchive())
     {
         archive.CreateEntry("entry1.bin", provider, new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings(), new SevenZipAESEncryptionSettings("test1"))); 
         archive.Save(sevenZipFile);
     }
 }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| имя | java.lang.String | Имя записи. |
| streamProvider | java.util.function.Supplier&lt;java.io.InputStream&gt; | Метод, предоставляющий поток ввода для записи. |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - SevenZip entry instance.
### createEntry(String name, Supplier&lt;InputStream&gt; streamProvider, SevenZipEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--com.aspose.zip.SevenZipEntrySettings-}
```
public final SevenZipArchiveEntry createEntry(String name, Supplier<InputStream> streamProvider, SevenZipEntrySettings newEntrySettings)
```


Создайте одну запись в архиве.

Создайте архив с записью, сжатой LZMA2 и зашифрованной.

```

``````

System.Func&lt;Stream&gt; provider = delegate(){ return new MemoryStream(new byte[]{0xFF, 0x00}); };
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
using (var archive = new SevenZipArchive())
{
archive.CreateEntry("entry1.bin", provider, new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings(), new SevenZipAESEncryptionSettings("test1")));
archive.Save(sevenZipFile);
}
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| streamProvider | java.util.function.Supplier&lt;java.io.InputStream&gt; | The method providing input stream for the entry. |
| newEntrySettings | [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) | Compression and encryption settings used for added [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) item. Individual compression settings is ignored in case of solid compression, see `SevenZipEntrySettings.Solid`([SevenZipEntrySettings.getSolid](../../com.aspose.zip/sevenzipentrysettings\#getSolid)/[SevenZipEntrySettings.setSolid](../../com.aspose.zip/sevenzipentrysettings\#setSolid)). |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - SevenZip entry instance.
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all the files in the archive to the directory provided.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
         archive.extractToDirectory("C:\\extracted");
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | destinationDirectory | java.lang.String | путь к каталогу, в который будут помещены извлечённые файлы. |

Если каталог не существует, он будет создан |

### extractToDirectory(String destinationDirectory, String password) {#extractToDirectory-java.lang.String-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory, String password)
```


Извлекает все файлы из архива в указанный каталог.

```

``````

try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
archive.extractToDirectory("C:\\extracted");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in

If the directory does not exist, it will be created. |
| password | java.lang.String | optional password for content decryption.

`password` is used for content decryption only. If file names are encrypted provide password in [SevenZipArchive(String, String)](../../com.aspose.zip/sevenziparchive\#SevenZipArchive-String--String-) or [SevenZipArchive(java.io.InputStream, String)](../../com.aspose.zip/sevenziparchive\#SevenZipArchive-java.io.InputStream--String-) constructor. |

### getEntries() {#getEntries--}
```
public final List<SevenZipArchiveEntry> getEntries()
```


Gets entries of [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) type constituting the archive.

**Returns:**
java.util.List&lt;com.aspose.zip.SevenZipArchiveEntry&gt; - entries of [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) type constituting the archive
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the 7z archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the 7z archive
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Gets the archive format.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getNewEntrySettings() {#getNewEntrySettings--}
```
public final SevenZipEntrySettings getNewEntrySettings()
```


Compression and encryption settings used for newly added [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) items.

**Returns:**
[SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) - compression and encryption settings used for newly added [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) items
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves 7z archive to the stream provided.

```

``````

     try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (SevenZipArchive archive = new SevenZipArchive()) {
                 archive.createEntry("data", source);
                 archive.save(sevenZipFile);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| output | java.io.OutputStream | поток назначения |

### save(OutputStream output, SevenZipArchiveSaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.SevenZipArchiveSaveOptions-}
```
public final void save(OutputStream output, SevenZipArchiveSaveOptions saveOptions)
```


Сохраняет архив 7z в предоставленный поток.

```

``````

try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (SevenZipArchive archive = new SevenZipArchive()) {
archive.createEntry("data", source);
archive.save(sevenZipFile);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream |
| saveOptions | [SevenZipArchiveSaveOptions](../../com.aspose.zip/sevenziparchivesaveoptions) | Options for archive saving. |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves archive to a destination file provided.

```

``````

  using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
  {
     using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings())))
     {
        archive.CreateEntry("data", source);
        archive.Save("archive.7z");
     }
  }
  
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | destinationFileName | java.lang.String | Путь к создаваемому архиву. Если указанный файл уже существует, он будет перезаписан. |

Можно сохранить архив в тот же путь, из которого он был загружен. Однако это не рекомендуется, потому что такой подход использует копирование во временный файл. |

### save(String destinationFileName, SevenZipArchiveSaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.SevenZipArchiveSaveOptions-}
```
public final void save(String destinationFileName, SevenZipArchiveSaveOptions saveOptions)
```


Сохраняет архив в указанный файл назначения.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings()))) {
archive.createEntry("data", source);
archive.save("archive.7z");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |
| saveOptions | [SevenZipArchiveSaveOptions](../../com.aspose.zip/sevenziparchivesaveoptions) | Options for archive saving.

It is possible to save an archive to the same path as it was loaded from. However, this is not recommended because this approach uses copying to a temporary file. |

### saveSplit(String destinationDirectory, SplitSevenZipArchiveSaveOptions options) {#saveSplit-java.lang.String-com.aspose.zip.SplitSevenZipArchiveSaveOptions-}
```
public final void saveSplit(String destinationDirectory, SplitSevenZipArchiveSaveOptions options)
```


Saves multi-volume archive to destination directory provided.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive()) {
         archive.createEntry("entry.bin", "data.bin");
         archive.saveSplit("C:\\Folder", new SplitSevenZipArchiveSaveOptions("volume", 65536));
     }
 
```

Этот метод собирает несколько файлов `(n)` filename.7z.001, filename.7z.002, ..., filename.7z.(n).

Невозможно сделать существующий архив многотомным.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| destinationDirectory | java.lang.String | путь к каталогу, в котором будут создаваться сегменты архива |
| options | [SplitSevenZipArchiveSaveOptions](../../com.aspose.zip/splitsevenziparchivesaveoptions) | опции сохранения архива, включая имя файла |

