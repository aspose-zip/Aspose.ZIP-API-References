---
title: "TarArchive"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Этот класс представляет файл архива tar."
type: docs
weight: 125
url: /ru/java/com.aspose.zip/tararchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class TarArchive implements IArchive, AutoCloseable
```

Этот класс представляет файл tar-архива. Используйте его для создания, извлечения или обновления tar-архивов.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [TarArchive()](#TarArchive--) | Инициализирует новый экземпляр класса [TarArchive](../../com.aspose.zip/tararchive). |
| [TarArchive(InputStream sourceStream)](#TarArchive-java.io.InputStream-) | Инициализирует новый экземпляр класса [Archive](../../com.aspose.zip/archive) и формирует список записей, которые можно извлечь из архива. |
| [TarArchive(String path)](#TarArchive-java.lang.String-) | Инициализирует новый экземпляр класса [TarArchive](../../com.aspose.zip/tararchive) и формирует список записей, которые можно извлечь из архива. |
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
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | Создаёт одну запись внутри архива. |
| [createEntry(String name, InputStream source, File file)](#createEntry-java.lang.String-java.io.InputStream-java.io.File-) | Создаёт одну запись внутри архива. |
| [createEntry(String name, String path)](#createEntry-java.lang.String-java.lang.String-) | Создаёт одну запись внутри архива. |
| [createEntry(String name, String path, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | Создаёт одну запись внутри архива. |
| [deleteEntry(TarEntry entry)](#deleteEntry-com.aspose.zip.TarEntry-) | Удаляет первое вхождение конкретной записи из списка записей. |
| [deleteEntry(int entryIndex)](#deleteEntry-int-) | Удаляет запись из списка записей по индексу. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Извлекает все файлы из архива в указанный каталог. |
| [fromGZip(InputStream source)](#fromGZip-java.io.InputStream-) | Извлекает предоставленный gzip-архив и создает [TarArchive](../../com.aspose.zip/tararchive) из извлеченных данных. |
| [fromGZip(String path)](#fromGZip-java.lang.String-) | Извлекает предоставленный gzip-архив и создает [TarArchive](../../com.aspose.zip/tararchive) из извлеченных данных. |
| [fromLZ4(InputStream source)](#fromLZ4-java.io.InputStream-) | Извлекает предоставленный LZ4-архив и создает [TarArchive](../../com.aspose.zip/tararchive) из извлеченных данных. |
| [fromLZ4(String path)](#fromLZ4-java.lang.String-) | Извлекает предоставленный LZ4-архив и создает [TarArchive](../../com.aspose.zip/tararchive) из извлеченных данных. |
| [fromLZMA(InputStream source)](#fromLZMA-java.io.InputStream-) | Извлекает предоставленный LZMA-архив и создает [TarArchive](../../com.aspose.zip/tararchive) из извлеченных данных. |
| [fromLZMA(String path)](#fromLZMA-java.lang.String-) | Извлекает предоставленный LZMA-архив и создает [TarArchive](../../com.aspose.zip/tararchive) из извлеченных данных. |
| [fromLZip(InputStream source)](#fromLZip-java.io.InputStream-) | Извлекает предоставленный lzip-архив и создает [TarArchive](../../com.aspose.zip/tararchive) из извлеченных данных. |
| [fromLZip(String path)](#fromLZip-java.lang.String-) | Извлекает предоставленный lzip-архив и создает [TarArchive](../../com.aspose.zip/tararchive) из извлеченных данных. |
| [fromXz(InputStream source)](#fromXz-java.io.InputStream-) | Извлекает предоставленный архив формата xz и создает [TarArchive](../../com.aspose.zip/tararchive) из извлеченных данных. |
| [fromXz(String path)](#fromXz-java.lang.String-) | Извлекает предоставленный архив формата xz и создает [TarArchive](../../com.aspose.zip/tararchive) из извлеченных данных. |
| [fromZ(InputStream source)](#fromZ-java.io.InputStream-) | Извлекает предоставленный архив формата Z и создает [TarArchive](../../com.aspose.zip/tararchive) из извлеченных данных. |
| [fromZ(String path)](#fromZ-java.lang.String-) | Извлекает предоставленный архив формата Z и создает [TarArchive](../../com.aspose.zip/tararchive) из извлеченных данных. |
| [fromZstandard(InputStream source)](#fromZstandard-java.io.InputStream-) | Извлекает предоставленный Zstandard-архив и создает [TarArchive](../../com.aspose.zip/tararchive) из извлеченных данных. |
| [fromZstandard(String path)](#fromZstandard-java.lang.String-) | Извлекает предоставленный Zstandard-архив и создает [TarArchive](../../com.aspose.zip/tararchive) из извлеченных данных. |
| [getEntries()](#getEntries--) | Получает записи типа [TarEntry](../../com.aspose.zip/tarentry), составляющие архив. |
| [getFileEntries()](#getFileEntries--) | Получает записи типа [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), составляющие tar-архив. |
| [getFormat()](#getFormat--) | Получает формат архива. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Сохраняет архив в предоставленный поток. |
| [save(OutputStream output, TarFormat format)](#save-java.io.OutputStream-com.aspose.zip.TarFormat-) | Сохраняет архив в предоставленный поток. |
| [save(String destinationFileName)](#save-java.lang.String-) | Сохраняет архив в указанный файл назначения. |
| [save(String destinationFileName, TarFormat format)](#save-java.lang.String-com.aspose.zip.TarFormat-) | Сохраняет архив в указанный файл назначения. |
| [saveGzipped(OutputStream output)](#saveGzipped-java.io.OutputStream-) | Сохраняет архив в поток с gzip‑сжатием. |
| [saveGzipped(OutputStream output, TarFormat format)](#saveGzipped-java.io.OutputStream-com.aspose.zip.TarFormat-) | Сохраняет архив в поток с gzip‑сжатием. |
| [saveGzipped(String path)](#saveGzipped-java.lang.String-) | Сохраняет архив в файл по пути с gzip‑сжатием. |
| [saveGzipped(String path, TarFormat format)](#saveGzipped-java.lang.String-com.aspose.zip.TarFormat-) | Сохраняет архив в файл по пути с gzip‑сжатием. |
| [saveLZ4Compressed(OutputStream output)](#saveLZ4Compressed-java.io.OutputStream-) | Сохраняет архив в поток с сжатием LZ4. |
| [saveLZ4Compressed(OutputStream output, TarFormat format)](#saveLZ4Compressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | Сохраняет архив в поток с сжатием LZ4. |
| [saveLZ4Compressed(String path)](#saveLZ4Compressed-java.lang.String-) | Сохраняет архив в файл по пути с сжатием LZ4. |
| [saveLZ4Compressed(String path, TarFormat format)](#saveLZ4Compressed-java.lang.String-com.aspose.zip.TarFormat-) | Сохраняет архив в файл по пути с сжатием LZ4. |
| [saveLZMACompressed(OutputStream output)](#saveLZMACompressed-java.io.OutputStream-) | Сохраняет архив в поток с сжатием LZMA. |
| [saveLZMACompressed(OutputStream output, TarFormat format)](#saveLZMACompressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | Сохраняет архив в поток с сжатием LZMA. |
| [saveLZMACompressed(String path)](#saveLZMACompressed-java.lang.String-) | Сохраняет архив в файл по пути с сжатием lzma. |
| [saveLZMACompressed(String path, TarFormat format)](#saveLZMACompressed-java.lang.String-com.aspose.zip.TarFormat-) | Сохраняет архив в файл по пути с сжатием lzma. |
| [saveLzipped(OutputStream output)](#saveLzipped-java.io.OutputStream-) | Сохраняет архив в поток с lzip‑сжатием. |
| [saveLzipped(OutputStream output, TarFormat format)](#saveLzipped-java.io.OutputStream-com.aspose.zip.TarFormat-) | Сохраняет архив в поток с lzip‑сжатием. |
| [saveLzipped(String path)](#saveLzipped-java.lang.String-) | Сохраняет архив в файл по пути с lzip‑сжатием. |
| [saveLzipped(String path, TarFormat format)](#saveLzipped-java.lang.String-com.aspose.zip.TarFormat-) | Сохраняет архив в файл по пути с lzip‑сжатием. |
| [saveXzCompressed(OutputStream output)](#saveXzCompressed-java.io.OutputStream-) | Сохраняет архив в поток с xz‑сжатием. |
| [saveXzCompressed(OutputStream output, TarFormat format)](#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | Сохраняет архив в поток с xz‑сжатием. |
| [saveXzCompressed(OutputStream output, TarFormat format, XzArchiveSettings settings)](#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-) | Сохраняет архив в поток с xz‑сжатием. |
| [saveXzCompressed(String path)](#saveXzCompressed-java.lang.String-) | Сохраняет архив в файл по пути с xz‑сжатием. |
| [saveXzCompressed(String path, TarFormat format)](#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-) | Сохраняет архив в файл по пути с xz‑сжатием. |
| [saveXzCompressed(String path, TarFormat format, XzArchiveSettings settings)](#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-) | Сохраняет архив в файл по пути с xz‑сжатием. |
| [saveZCompressed(OutputStream output)](#saveZCompressed-java.io.OutputStream-) | Сохраняет архив в поток с Z‑сжатием. |
| [saveZCompressed(OutputStream output, TarFormat format)](#saveZCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | Сохраняет архив в поток с Z‑сжатием. |
| [saveZCompressed(String path)](#saveZCompressed-java.lang.String-) | Сохраняет архив в файл по пути с Z‑сжатием. |
| [saveZCompressed(String path, TarFormat format)](#saveZCompressed-java.lang.String-com.aspose.zip.TarFormat-) | Сохраняет архив в файл по пути с Z‑сжатием. |
| [saveZstandard(OutputStream output)](#saveZstandard-java.io.OutputStream-) | Сохраняет архив в поток с Zstandard‑сжатием. |
| [saveZstandard(OutputStream output, TarFormat format)](#saveZstandard-java.io.OutputStream-com.aspose.zip.TarFormat-) | Сохраняет архив в поток с Zstandard‑сжатием. |
| [saveZstandard(String path)](#saveZstandard-java.lang.String-) | Сохраняет архив в файл по пути с Zstandard‑сжатием. |
| [saveZstandard(String path, TarFormat format)](#saveZstandard-java.lang.String-com.aspose.zip.TarFormat-) | Сохраняет архив в файл по пути с Zstandard‑сжатием. |
### TarArchive() {#TarArchive--}
```
public TarArchive()
```


Инициализирует новый экземпляр класса [TarArchive](../../com.aspose.zip/tararchive).

Следующий пример показывает, как сжать файл.

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry(first.bin, \"data.bin\");
archive.save("archive.tar");
}
 
```



### TarArchive(InputStream sourceStream) {#TarArchive-java.io.InputStream-}
```
public TarArchive(InputStream sourceStream)
```


Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (TarArchive archive = new TarArchive(new FileInputStream("archive.tar"))) {
             archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

Этот конструктор не распаковывает ни одну запись. См. метод [TarEntry.open()](../../com.aspose.zip/tarentry\\#open--) для распаковки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceStream | java.io.InputStream | источник архива |

### TarArchive(String path) {#TarArchive-java.lang.String-}
```
public TarArchive(String path)
```


Инициализирует новый экземпляр класса [TarArchive](../../com.aspose.zip/tararchive) и формирует список записей, которые можно извлечь из архива.

В следующем примере показано, как извлечь все записи в каталог.

```

``````

try (TarArchive archive = new TarArchive("archive.tar")) {
archive.extractToDirectory("C:\\extracted");
}
 
```

This constructor does not unpack any entry. See [TarEntry.open()](../../com.aspose.zip/tarentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final TarArchive createEntries(File directory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntries(new java.io.File("C:\\folder"), false);
             archive.save(tarFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| directory | java.io.File | директория для сжатия |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final TarArchive createEntries(File directory, boolean includeRootDirectory)
```


Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога.

```

``````

try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntries(new java.io.File("C:\\folder"), false);
archive.save(tarFile);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntries(String sourceDirectory) {#createEntries-java.lang.String-}
```
public final TarArchive createEntries(String sourceDirectory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntries("C:\\folder", false);
             archive.save(tarFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceDirectory | java.lang.String | директория для сжатия |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntries(String sourceDirectory, boolean includeRootDirectory) {#createEntries-java.lang.String-boolean-}
```
public final TarArchive createEntries(String sourceDirectory, boolean includeRootDirectory)
```


Добавляет в архив все файлы и каталоги рекурсивно из указанного каталога.

```

``````

try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntries("C:\\folder", false);
archive.save(tarFile);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntry(String name, File file) {#createEntry-java.lang.String-java.io.File-}
```
public final TarEntry createEntry(String name, File file)
```


Creates a single entry within the archive.

```

``````

     File fi = new File("data.bin");
     try (TarArchive archive = new TarArchive()) {
         archive.createEntry("data.bin", fi);
         archive.save(tarFile);
     }
 
```

Имя записи задаётся исключительно параметром `name`. Имя файла, переданное в параметре `file`, не влияет на имя записи.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| имя | java.lang.String | имя элемента |
| file | java.io.File | метаданные файла или папки, которые будут сжаты |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, File file, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final TarEntry createEntry(String name, File file, boolean openImmediately)
```


Создаёт одну запись внутри архива.

```

``````

File fi = new File("data.bin");
try (TarArchive archive = new TarArchive()) {
archive.createEntry("data.bin", fi);
archive.save(tarFile);
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `file` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is disposed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file or folder to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final TarEntry createEntry(String name, InputStream source)
```


Creates a single entry within the archive.

```

``````

     try (TarArchive archive = new TarArchive()) {
         archive.createEntry("bytes", new ByteArrayInputStream(new byte[] {0x00, (byte) 0xFF}));
         archive.save(tarFile);
     }
 
```

Имя записи задаётся исключительно параметром `name`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| имя | java.lang.String | имя элемента |
| source | java.io.InputStream | входной поток для записи |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, InputStream source, File file) {#createEntry-java.lang.String-java.io.InputStream-java.io.File-}
```
public final TarEntry createEntry(String name, InputStream source, File file)
```


Создаёт одну запись внутри архива.

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry("bytes", new ByteArrayInputStream(new byte[] {0x00, (byte) 0xFF}));
archive.save(tarFile);
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `file` parameter does not affect the entry name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| source | java.io.InputStream | the input stream for the entry |
| file | java.io.File | the metadata of file or folder to be compressed |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, String path) {#createEntry-java.lang.String-java.lang.String-}
```
public final TarEntry createEntry(String name, String path)
```


Creates a single entry within the archive.

```

``````

     try (TarArchive archive = new TarArchive()) {
             archive.createEntry(first.bin, "data.bin");
             archive.save(outputTarFile);
     }
 
```

Имя элемента задаётся исключительно параметром `name`. Имя файла, переданное в параметре `path`, не влияет на имя элемента.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| имя | java.lang.String | имя элемента |
| path | java.lang.String | путь к файлу для сжатия |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, String path, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final TarEntry createEntry(String name, String path, boolean openImmediately)
```


Создаёт одну запись внутри архива.

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry(first.bin, \"data.bin\");
archive.save(outputTarFile);
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `path` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is disposed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| path | java.lang.String | path to file to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### deleteEntry(TarEntry entry) {#deleteEntry-com.aspose.zip.TarEntry-}
```
public final TarArchive deleteEntry(TarEntry entry)
```


Removes the first occurrence of a specific entry from the entry list.

Here is how you can remove all entries except the last one:

```

``````

     try (TarArchive archive = new TarArchive("archive.tar")) {
         while (archive.getEntries().size() > 1)
             archive.deleteEntry(archive.getEntries().get_Item(0));
         archive.save(outputTarFile);
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| entry | [TarEntry](../../com.aspose.zip/tarentry) | запись, которую нужно удалить из списка записей |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with the entry deleted
### deleteEntry(int entryIndex) {#deleteEntry-int-}
```
public final TarArchive deleteEntry(int entryIndex)
```


Удаляет запись из списка записей по индексу.

```

``````

try (TarArchive archive = new TarArchive("two_files.tar")) {
archive.deleteEntry(0);
archive.save("single_file.tar");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| entryIndex | int | the zero-based index of the entry to remove |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with the entry deleted
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all the files in the archive to the directory provided.

```

``````

     try (TarArchive archive = new TarArchive("archive.tar")) {
         archive.extractToDirectory("C:\\extracted");
     }
 
```

Если каталог не существует, он будет создан.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| destinationDirectory | java.lang.String | путь к каталогу, в который будут помещены извлечённые файлы |

### fromGZip(InputStream source) {#fromGZip-java.io.InputStream-}
```
public static TarArchive fromGZip(InputStream source)
```


Извлекает предоставленный gzip-архив и создает [TarArchive](../../com.aspose.zip/tararchive) из извлеченных данных.

Важно: gzip‑архив полностью извлекается в этом методе, его содержимое хранится во внутренней памяти. Будьте внимательны к потреблению памяти.

Поток извлечения GZip не поддерживает перемещение, что обусловлено природой алгоритма сжатия. Tar‑архив предоставляет возможность извлекать произвольные записи, поэтому ему требуется работать с перемещаемым потоком в реализации.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| source | java.io.InputStream | источник архива. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromGZip(String path) {#fromGZip-java.lang.String-}
```
public static TarArchive fromGZip(String path)
```


Извлекает предоставленный gzip-архив и создает [TarArchive](../../com.aspose.zip/tararchive) из извлеченных данных.

Важно: gzip‑архив полностью извлекается в этом методе, его содержимое хранится во внутренней памяти. Будьте внимательны к потреблению памяти.

Поток извлечения GZip не поддерживает перемещение, что обусловлено природой алгоритма сжатия. Tar‑архив предоставляет возможность извлекать произвольные записи, поэтому ему требуется работать с перемещаемым потоком в реализации.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| path | java.lang.String | путь к файлу архива. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZ4(InputStream source) {#fromLZ4-java.io.InputStream-}
```
public static TarArchive fromLZ4(InputStream source)
```


Извлекает предоставленный LZ4-архив и создает [TarArchive](../../com.aspose.zip/tararchive) из извлеченных данных.

Важно: LZ4‑архив полностью извлекается в этом методе, его содержимое хранится во внутренней памяти. Будьте внимательны к потреблению памяти.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | source | java.io.InputStream | Источник архива. |

Поток извлечения LZ4 не поддерживает перемещение из‑за природы алгоритма сжатия. Архив Tar предоставляет возможность извлекать произвольные записи, поэтому он должен работать с поддерживаемым перемещением потоком в основе. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - An instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZ4(String path) {#fromLZ4-java.lang.String-}
```
public static TarArchive fromLZ4(String path)
```


Извлекает предоставленный LZ4-архив и создает [TarArchive](../../com.aspose.zip/tararchive) из извлеченных данных.

Важно: LZ4‑архив полностью извлекается в этом методе, его содержимое хранится во внутренней памяти. Будьте внимательны к потреблению памяти.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | path | java.lang.String | Путь к файлу архива. |

Поток извлечения LZ4 не поддерживает перемещение из‑за природы алгоритма сжатия. Архив Tar предоставляет возможность извлекать произвольные записи, поэтому он должен работать с поддерживаемым перемещением потоком в основе. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - An instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZMA(InputStream source) {#fromLZMA-java.io.InputStream-}
```
public static TarArchive fromLZMA(InputStream source)
```


Извлекает предоставленный LZMA-архив и создает [TarArchive](../../com.aspose.zip/tararchive) из извлеченных данных.

Важно: архив LZMA полностью извлекается в этом методе, его содержимое хранится внутри. Будьте внимательны к потреблению памяти.

Поток извлечения LZMA не поддерживает перемещение из‑за природы алгоритма сжатия. Архив Tar предоставляет возможность извлекать произвольные записи, поэтому он должен работать с поддерживаемым перемещением потоком в основе.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| source | java.io.InputStream | источник архива |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZMA(String path) {#fromLZMA-java.lang.String-}
```
public static TarArchive fromLZMA(String path)
```


Извлекает предоставленный LZMA-архив и создает [TarArchive](../../com.aspose.zip/tararchive) из извлеченных данных.

Важно: архив LZMA полностью извлекается в этом методе, его содержимое хранится внутри. Будьте внимательны к потреблению памяти.

Поток извлечения LZMA не поддерживает перемещение из‑за природы алгоритма сжатия. Архив Tar предоставляет возможность извлекать произвольные записи, поэтому он должен работать с поддерживаемым перемещением потоком в основе.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| path | java.lang.String | путь к файлу архива |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZip(InputStream source) {#fromLZip-java.io.InputStream-}
```
public static TarArchive fromLZip(InputStream source)
```


Извлекает предоставленный lzip-архив и создает [TarArchive](../../com.aspose.zip/tararchive) из извлеченных данных.

Важно: архив lzip полностью извлекается в этом методе, его содержимое хранится внутри. Будьте внимательны к потреблению памяти.

Поток извлечения Lzip не поддерживает перемещение из‑за природы алгоритма сжатия. Архив Tar предоставляет возможность извлекать произвольные записи, поэтому он должен работать с поддерживаемым перемещением потоком в основе.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| source | java.io.InputStream | источник архива. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZip(String path) {#fromLZip-java.lang.String-}
```
public static TarArchive fromLZip(String path)
```


Извлекает предоставленный lzip-архив и создает [TarArchive](../../com.aspose.zip/tararchive) из извлеченных данных.

Важно: архив lzip полностью извлекается в этом методе, его содержимое хранится внутри. Будьте внимательны к потреблению памяти.

Поток извлечения Lzip не поддерживает перемещение из‑за природы алгоритма сжатия. Архив Tar предоставляет возможность извлекать произвольные записи, поэтому он должен работать с поддерживаемым перемещением потоком в основе.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| path | java.lang.String | путь к файлу архива. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromXz(InputStream source) {#fromXz-java.io.InputStream-}
```
public static TarArchive fromXz(InputStream source)
```


Извлекает предоставленный архив формата xz и создает [TarArchive](../../com.aspose.zip/tararchive) из извлеченных данных.

Важно: архив xz полностью извлекается в этом методе, его содержимое хранится внутри. Будьте внимательны к потреблению памяти.

Архив Tar предоставляет возможность извлекать произвольные записи, поэтому он должен работать с поддерживаемым перемещением потоком в основе.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| source | java.io.InputStream | источник архива |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromXz(String path) {#fromXz-java.lang.String-}
```
public static TarArchive fromXz(String path)
```


Извлекает предоставленный архив формата xz и создает [TarArchive](../../com.aspose.zip/tararchive) из извлеченных данных.

Важно: архив xz полностью извлекается в этом методе, его содержимое хранится внутри. Будьте внимательны к потреблению памяти.

Архив Tar предоставляет возможность извлекать произвольные записи, поэтому он должен работать с поддерживаемым перемещением потоком в основе.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| path | java.lang.String | путь к файлу архива |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZ(InputStream source) {#fromZ-java.io.InputStream-}
```
public static TarArchive fromZ(InputStream source)
```


Извлекает предоставленный архив формата Z и создает [TarArchive](../../com.aspose.zip/tararchive) из извлеченных данных.

Важно: архив Z полностью извлекается в этом методе, его содержимое хранится внутри. Будьте внимательны к потреблению памяти.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| source | java.io.InputStream | источник архива |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZ(String path) {#fromZ-java.lang.String-}
```
public static TarArchive fromZ(String path)
```


Извлекает предоставленный архив формата Z и создает [TarArchive](../../com.aspose.zip/tararchive) из извлеченных данных.

Важно: архив Z полностью извлекается в этом методе, его содержимое хранится внутри. Будьте внимательны к потреблению памяти.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| path | java.lang.String | путь к файлу архива |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZstandard(InputStream source) {#fromZstandard-java.io.InputStream-}
```
public static TarArchive fromZstandard(InputStream source)
```


Извлекает предоставленный Zstandard-архив и создает [TarArchive](../../com.aspose.zip/tararchive) из извлеченных данных.

Важно: архив Zstandard полностью извлекается в этом методе, его содержимое хранится внутри. Будьте внимательны к потреблению памяти.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| source | java.io.InputStream | источник архива |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZstandard(String path) {#fromZstandard-java.lang.String-}
```
public static TarArchive fromZstandard(String path)
```


Извлекает предоставленный Zstandard-архив и создает [TarArchive](../../com.aspose.zip/tararchive) из извлеченных данных.

Важно: архив Zstandard полностью извлекается в этом методе, его содержимое хранится внутри. Будьте внимательны к потреблению памяти.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| path | java.lang.String | путь к файлу архива |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### getEntries() {#getEntries--}
```
public final List<TarEntry> getEntries()
```


Получает записи типа [TarEntry](../../com.aspose.zip/tarentry), составляющие архив.

**Returns:**
java.util.List&lt;com.aspose.zip.TarEntry&gt; - элементы типа [TarEntry](../../com.aspose.zip/tarentry), составляющие архив
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Получает записи типа [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), составляющие tar-архив.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - элементы типа [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), составляющие tar‑архив
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

```

``````

try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry1", "data.bin");
archive.save(tarFile);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### save(OutputStream output, TarFormat format) {#save-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void save(OutputStream output, TarFormat format)
```


Saves archive to the stream provided.

```

``````

     try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry1", "data.bin");
             archive.save(tarFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | output | java.io.OutputStream | целевой поток. |

`output` должен быть доступен для записи |
| format | [TarFormat](../../com.aspose.zip/tarformat) | определяет формат заголовка tar. Значение null будет рассматриваться как USTar, когда это возможно |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Сохраняет архив в указанный файл назначения.

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry1", "data.bin");
archive.save("myarchive.tar");
}
 
```

It is possible to save an archive to the same path as it was loaded from. However, this is not recommended because this approach uses copying to a temporary file

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |

### save(String destinationFileName, TarFormat format) {#save-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void save(String destinationFileName, TarFormat format)
```


Saves archive to the destination file provided.

```

``````

     try (TarArchive archive = new TarArchive()) {
         archive.createEntry("entry1", "data.bin");
         archive.save("myarchive.tar");
     }
 
```

Можно сохранить архив в тот же путь, из которого он был загружен. Однако это не рекомендуется, потому что такой подход использует копирование во временный файл

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| destinationFileName | java.lang.String | путь к архиву, который будет создан. Если указанный файл уже существует, он будет перезаписан. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | определяет формат заголовка tar. Значение null будет рассматриваться как USTar, когда это возможно |

### saveGzipped(OutputStream output) {#saveGzipped-java.io.OutputStream-}
```
public final void saveGzipped(OutputStream output)
```


Сохраняет архив в поток с gzip‑сжатием.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.gz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveGzipped(result);
}
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### saveGzipped(OutputStream output, TarFormat format) {#saveGzipped-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveGzipped(OutputStream output, TarFormat format)
```


Saves archive to the stream with gzip compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.gz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveGzipped(result);
             }
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | output | java.io.OutputStream | целевой поток. |

`output` должен быть доступен для записи |
| format | [TarFormat](../../com.aspose.zip/tarformat) | определяет формат заголовка tar. Значение null будет рассматриваться как USTar, когда это возможно |

### saveGzipped(String path) {#saveGzipped-java.lang.String-}
```
public final void saveGzipped(String path)
```


Сохраняет архив в файл по пути с gzip‑сжатием.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveGzipped("result.tar.gz");
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveGzipped(String path, TarFormat format) {#saveGzipped-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveGzipped(String path, TarFormat format)
```


Saves archive to the file by path with gzip compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveGzipped("result.tar.gz");
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| path | java.lang.String | путь к создаваемому архиву. Если указанный файл уже существует, он будет перезаписан |
| format | [TarFormat](../../com.aspose.zip/tarformat) | определяет формат заголовка tar. Значение null будет рассматриваться как USTar, когда это возможно |

### saveLZ4Compressed(OutputStream output) {#saveLZ4Compressed-java.io.OutputStream-}
```
public final void saveLZ4Compressed(OutputStream output)
```


Сохраняет архив в поток с сжатием LZ4.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.lz4")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZ4Compressed(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | Destination stream. |

### saveLZ4Compressed(OutputStream output, TarFormat format) {#saveLZ4Compressed-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveLZ4Compressed(OutputStream output, TarFormat format)
```


Saves archive to the stream with LZ4 compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.lz4")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveLZ4Compressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| output | java.io.OutputStream | Поток назначения. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | Определяет формат заголовка tar. Значение null будет рассматриваться как USTar, когда это возможно. |

### saveLZ4Compressed(String path) {#saveLZ4Compressed-java.lang.String-}
```
public final void saveLZ4Compressed(String path)
```


Сохраняет архив в файл по пути с сжатием LZ4.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZ4Compressed("result.tar.lz4");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |

### saveLZ4Compressed(String path, TarFormat format) {#saveLZ4Compressed-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveLZ4Compressed(String path, TarFormat format)
```


Saves archive to the file by path with LZ4 compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveLZ4Compressed("result.tar.lz4");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| path | java.lang.String | Путь к создаваемому архиву. Если указанный файл уже существует, он будет перезаписан. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | Определяет формат заголовка tar. Значение null будет рассматриваться как USTar, когда это возможно. |

### saveLZMACompressed(OutputStream output) {#saveLZMACompressed-java.io.OutputStream-}
```
public final void saveLZMACompressed(OutputStream output)
```


Сохраняет архив в поток с сжатием LZMA.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.lzma")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZMACompressed(result);
}
}
} catch (IOException ex) {
}
 
```

Important: tar archive is composed then compressed within this method, its content is kept internally. Beware of memory consumption.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### saveLZMACompressed(OutputStream output, TarFormat format) {#saveLZMACompressed-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveLZMACompressed(OutputStream output, TarFormat format)
```


Saves archive to the stream with LZMA compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.lzma")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveLZMACompressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```

Важно: tar‑архив создаётся, а затем сжимается внутри этого метода, его содержимое хранится внутренне. Будьте осторожны с потреблением памяти.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | output | java.io.OutputStream | целевой поток. |

`output` должен быть доступен для записи |
| format | [TarFormat](../../com.aspose.zip/tarformat) | определяет формат заголовка tar. Значение null будет рассматриваться как USTar, когда это возможно |

### saveLZMACompressed(String path) {#saveLZMACompressed-java.lang.String-}
```
public final void saveLZMACompressed(String path)
```


Сохраняет архив в файл по пути с сжатием lzma.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZMACompressed("result.tar.lzma");
}
} catch (IOException ex) {
}
 
```

Important: tar archive is composed then compressed within this method, its content is kept internally. Beware of memory consumption.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveLZMACompressed(String path, TarFormat format) {#saveLZMACompressed-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveLZMACompressed(String path, TarFormat format)
```


Saves archive to the file by path with lzma compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveLZMACompressed("result.tar.lzma");
         }
     } catch (IOException ex) {
     }
 
```

Важно: tar‑архив создаётся, а затем сжимается внутри этого метода, его содержимое хранится внутренне. Будьте осторожны с потреблением памяти.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| path | java.lang.String | путь к создаваемому архиву. Если указанный файл уже существует, он будет перезаписан |
| format | [TarFormat](../../com.aspose.zip/tarformat) | определяет формат заголовка tar. Значение null будет рассматриваться как USTar, когда это возможно |

### saveLzipped(OutputStream output) {#saveLzipped-java.io.OutputStream-}
```
public final void saveLzipped(OutputStream output)
```


Сохраняет архив в поток с lzip‑сжатием.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.lz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLzipped(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### saveLzipped(OutputStream output, TarFormat format) {#saveLzipped-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveLzipped(OutputStream output, TarFormat format)
```


Saves archive to the stream with lzip compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.lz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveLzipped(result, TarFormat.Gnu);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | output | java.io.OutputStream | целевой поток. |

`output` должен быть доступен для записи |
| format | [TarFormat](../../com.aspose.zip/tarformat) | определяет формат заголовка tar. Значение null будет рассматриваться как USTar, когда это возможно |

### saveLzipped(String path) {#saveLzipped-java.lang.String-}
```
public final void saveLzipped(String path)
```


Сохраняет архив в файл по пути с lzip‑сжатием.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLzipped("result.tar.lz");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveLzipped(String path, TarFormat format) {#saveLzipped-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveLzipped(String path, TarFormat format)
```


Saves archive to the file by path with lzip compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveLzipped("result.tar.lz", TarFormat.Gnu);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| path | java.lang.String | путь к создаваемому архиву. Если указанный файл уже существует, он будет перезаписан |
| format | [TarFormat](../../com.aspose.zip/tarformat) | определяет формат заголовка tar. Значение null будет рассматриваться как USTar, когда это возможно |

### saveXzCompressed(OutputStream output) {#saveXzCompressed-java.io.OutputStream-}
```
public final void saveXzCompressed(OutputStream output)
```


Сохраняет архив в поток с xz‑сжатием.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.xz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveXzCompressed(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output`The stream must be writable |

### saveXzCompressed(OutputStream output, TarFormat format) {#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveXzCompressed(OutputStream output, TarFormat format)
```


Saves archive to the stream with xz compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.xz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveXzCompressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | output | java.io.OutputStream | целевой поток. |

`output`Поток должен быть доступен для записи |
| format | [TarFormat](../../com.aspose.zip/tarformat) | определяет формат заголовка tar. Значение null будет рассматриваться как USTar, когда это возможно |

### saveXzCompressed(OutputStream output, TarFormat format, XzArchiveSettings settings) {#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-}
```
public final void saveXzCompressed(OutputStream output, TarFormat format, XzArchiveSettings settings)
```


Сохраняет архив в поток с xz‑сжатием.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.xz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveXzCompressed(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output`The stream must be writable |
| format | [TarFormat](../../com.aspose.zip/tarformat) | defines the tar header format. Null value will be treated as USTar when possible |
| settings | [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) | set of setting particular xz archive: dictionary size, block size, check type |

### saveXzCompressed(String path) {#saveXzCompressed-java.lang.String-}
```
public final void saveXzCompressed(String path)
```


Saves archive to the file by path with xz compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveXzCompressed("result.tar.xz");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| path | java.lang.String | путь к создаваемому архиву. Если указанный файл уже существует, он будет перезаписан |

### saveXzCompressed(String path, TarFormat format) {#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveXzCompressed(String path, TarFormat format)
```


Сохраняет архив в файл по пути с xz‑сжатием.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveXzCompressed("result.tar.xz");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| format | [TarFormat](../../com.aspose.zip/tarformat) | defines tar header format. Null value will be treated as USTar when possible |

### saveXzCompressed(String path, TarFormat format, XzArchiveSettings settings) {#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-}
```
public final void saveXzCompressed(String path, TarFormat format, XzArchiveSettings settings)
```


Saves archive to the file by path with xz compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveXzCompressed("result.tar.xz");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| path | java.lang.String | путь к создаваемому архиву. Если указанный файл уже существует, он будет перезаписан |
| format | [TarFormat](../../com.aspose.zip/tarformat) | определяет формат заголовка tar. Значение null будет рассматриваться как USTar, когда это возможно |
| settings | [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) | набор параметров конкретного xz-архива: размер словаря, размер блока, тип проверки |

### saveZCompressed(OutputStream output) {#saveZCompressed-java.io.OutputStream-}
```
public final void saveZCompressed(OutputStream output)
```


Сохраняет архив в поток с Z‑сжатием.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.Z")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZCompressed(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | the destination stream |

### saveZCompressed(OutputStream output, TarFormat format) {#saveZCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveZCompressed(OutputStream output, TarFormat format)
```


Saves archive to the stream with Z compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.Z")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveZCompressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| output | java.io.OutputStream | поток назначения |
| format | [TarFormat](../../com.aspose.zip/tarformat) | определяет формат заголовка tar. Значение null будет рассматриваться как USTar, когда это возможно |

### saveZCompressed(String path) {#saveZCompressed-java.lang.String-}
```
public final void saveZCompressed(String path)
```


Сохраняет архив в файл по пути с Z‑сжатием.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZCompressed("result.tar.Z");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveZCompressed(String path, TarFormat format) {#saveZCompressed-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveZCompressed(String path, TarFormat format)
```


Saves archive to the file by path with Z compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveZCompressed("result.tar.Z");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| path | java.lang.String | путь к создаваемому архиву. Если указанный файл уже существует, он будет перезаписан |
| format | [TarFormat](../../com.aspose.zip/tarformat) | определяет формат заголовка tar. Значение null будет рассматриваться как USTar, когда это возможно |

### saveZstandard(OutputStream output) {#saveZstandard-java.io.OutputStream-}
```
public final void saveZstandard(OutputStream output)
```


Сохраняет архив в поток с Zstandard‑сжатием.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.zst")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZstandard(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### saveZstandard(OutputStream output, TarFormat format) {#saveZstandard-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveZstandard(OutputStream output, TarFormat format)
```


Saves archive to the stream with Zstandard compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.zst")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveZstandard(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | output | java.io.OutputStream | целевой поток. |

`output` должен быть доступен для записи |
| format | [TarFormat](../../com.aspose.zip/tarformat) | определяет формат заголовка tar. Значение null будет рассматриваться как USTar, когда это возможно |

### saveZstandard(String path) {#saveZstandard-java.lang.String-}
```
public final void saveZstandard(String path)
```


Сохраняет архив в файл по пути с Zstandard‑сжатием.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZstandard("result.tar.zst");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveZstandard(String path, TarFormat format) {#saveZstandard-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveZstandard(String path, TarFormat format)
```


Saves archive to the file by path with Zstandard compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveZstandard("result.tar.zst");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| path | java.lang.String | путь к создаваемому архиву. Если указанный файл уже существует, он будет перезаписан |
| format | [TarFormat](../../com.aspose.zip/tarformat) | определяет формат заголовка tar. Значение null будет рассматриваться как USTar, когда это возможно |

