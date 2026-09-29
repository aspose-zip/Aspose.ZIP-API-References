---
title: "RarArchive"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Этот класс представляет файл RAR-архива."
type: docs
weight: 97
url: /ru/java/com.aspose.zip/rararchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class RarArchive implements IArchive, AutoCloseable
```

Этот класс представляет файл RAR‑архива. Используйте его для извлечения RAR‑архивов.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [RarArchive(String path)](#RarArchive-java.lang.String-) | Инициализирует новый экземпляр класса [RarArchive](../../com.aspose.zip/rararchive) и формирует список записей, которые можно извлечь из архива. |
| [RarArchive(String path, RarArchiveLoadOptions loadOptions)](#RarArchive-java.lang.String-com.aspose.zip.RarArchiveLoadOptions-) | Инициализирует новый экземпляр класса [RarArchive](../../com.aspose.zip/rararchive) и формирует список записей, которые можно извлечь из архива. |
| [RarArchive(InputStream sourceStream)](#RarArchive-java.io.InputStream-) | Инициализирует новый экземпляр класса [RarArchive](../../com.aspose.zip/rararchive) и формирует список записей, которые можно извлечь из архива. |
| [RarArchive(InputStream sourceStream, RarArchiveLoadOptions loadOptions)](#RarArchive-java.io.InputStream-com.aspose.zip.RarArchiveLoadOptions-) | Инициализирует новый экземпляр класса [RarArchive](../../com.aspose.zip/rararchive) и формирует список записей, которые можно извлечь из архива. |
## Методы

| Метод | Описание |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Извлекает все файлы из архива в указанный каталог. |
| [getEntries()](#getEntries--) | Получает записи типа [RarArchiveEntry](../../com.aspose.zip/rararchiveentry), составляющие rar‑архив. |
| [getFileEntries()](#getFileEntries--) | Получает записи типа [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), составляющие rar‑архив. |
| [getFormat()](#getFormat--) | Получает формат архива. |
### RarArchive(String path) {#RarArchive-java.lang.String-}
```
public RarArchive(String path)
```


Инициализирует новый экземпляр класса [RarArchive](../../com.aspose.zip/rararchive) и формирует список записей, которые можно извлечь из архива.

В следующем примере архив извлекается, затем первая запись распаковывается в `MemoryStream`.

```

``````

ByteArrayOutputStream extracted = new ByteArrayOutputStream();
try (RarArchive archive = new RarArchive(\"data.rar\")) {
try (InputStream decompressed = archive.getEntries().get(0).open()) {
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
extracted.write(b, 0, bytesRead);
} catch (IOException ex) {
}
}
 
```

This constructor does not decompress any entry. See [RarArchiveEntry.open()](../../com.aspose.zip/rararchiveentry\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The fully qualified or the relative path to the archive file. |

### RarArchive(String path, RarArchiveLoadOptions loadOptions) {#RarArchive-java.lang.String-com.aspose.zip.RarArchiveLoadOptions-}
```
public RarArchive(String path, RarArchiveLoadOptions loadOptions)
```


Initializes a new instance of the [RarArchive](../../com.aspose.zip/rararchive) class and composes an entry list can be extracted from the archive.

The following example extracts an archive, then decompress first entry to a `MemoryStream`.

```

``````

     ByteArrayOutputStream extracted = new ByteArrayOutputStream();
     try (RarArchive archive = new RarArchive("data.rar")) {
         try (InputStream decompressed = archive.getEntries().get(0).open()) {
             byte[] b = new byte[8192];
             int bytesRead;
             while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
                 extracted.write(b, 0, bytesRead);
         } catch (IOException ex) {
         }
     }
 
```

Этот конструктор не распаковывает ни одну запись. См. метод [RarArchiveEntry.open()](../../com.aspose.zip/rararchiveentry\#open--) для распаковки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| path | java.lang.String | Полный или относительный путь к файлу архива. |
| loadOptions | [RarArchiveLoadOptions](../../com.aspose.zip/rararchiveloadoptions) | Параметры для загрузки существующего архива. |

### RarArchive(InputStream sourceStream) {#RarArchive-java.io.InputStream-}
```
public RarArchive(InputStream sourceStream)
```


Инициализирует новый экземпляр класса [RarArchive](../../com.aspose.zip/rararchive) и формирует список записей, которые можно извлечь из архива.


В следующем примере расшифровывается и распаковывается первая запись в `MemoryStream`.

```

``````

try (FileInputStream fs = new FileInputStream(\"encrypted.rar\")) {
ByteArrayOutputStream extracted = new ByteArrayOutputStream();
RarArchiveLoadOptions options = new RarArchiveLoadOptions();
options.setDecryptionPassword("p@s$");
try (RarArchive archive = new RarArchive(fs, options)) {
try (InputStream decompressed = archive.getEntries().get(0).open()) {
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
extracted.write(b, 0, bytesRead);
}
}
} catch (IOException ex) {
}
 
```

This constructor does not decompress any entry. See [RarArchiveEntry.open()](../../com.aspose.zip/rararchiveentry\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | The source of the archive. |

### RarArchive(InputStream sourceStream, RarArchiveLoadOptions loadOptions) {#RarArchive-java.io.InputStream-com.aspose.zip.RarArchiveLoadOptions-}
```
public RarArchive(InputStream sourceStream, RarArchiveLoadOptions loadOptions)
```


Initializes a new instance of the [RarArchive](../../com.aspose.zip/rararchive) class and composes an entry list can be extracted from the archive.


The following example decipher and decompress first entry to a `MemoryStream`.

```

``````

     try (FileInputStream fs = new FileInputStream("encrypted.rar")) {
         ByteArrayOutputStream extracted = new ByteArrayOutputStream();
         RarArchiveLoadOptions options = new RarArchiveLoadOptions();
         options.setDecryptionPassword("p@s$");
         try (RarArchive archive = new RarArchive(fs, options)) {
             try (InputStream decompressed = archive.getEntries().get(0).open()) {
                 byte[] b = new byte[8192];
                 int bytesRead;
                 while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
                     extracted.write(b, 0, bytesRead);
             }
         }
     } catch (IOException ex) {
     }
 
```

Этот конструктор не распаковывает ни одну запись. См. метод [RarArchiveEntry.open()](../../com.aspose.zip/rararchiveentry\#open--) для распаковки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| sourceStream | java.io.InputStream | Источник архива. |
| loadOptions | [RarArchiveLoadOptions](../../com.aspose.zip/rararchiveloadoptions) | Параметры для загрузки существующего архива. |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Извлекает все файлы из архива в указанный каталог.

```

``````

try (RarArchive archive = new RarArchive(\"archive.rar\")) {
archive.extractToDirectory("C:\\extracted");
}
 
```

If the directory does not exist, it will be created.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | The path to the directory to place the extracted files in. |

### getEntries() {#getEntries--}
```
public final List<RarArchiveEntry> getEntries()
```


Gets entries of [RarArchiveEntry](../../com.aspose.zip/rararchiveentry) type constituting the rar archive.

**Returns:**
java.util.List&lt;com.aspose.zip.RarArchiveEntry&gt; - entries of [RarArchiveEntry](../../com.aspose.zip/rararchiveentry) type constituting the rar archive.
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the rar archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the rar archive.
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Gets the archive format.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
