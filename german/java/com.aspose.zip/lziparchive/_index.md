---
title: "LzipArchive"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Diese Klasse stellt eine Lzip-Archivdatei dar."
type: docs
weight: 83
url: /de/java/com.aspose.zip/lziparchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class LzipArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

Diese Klasse stellt eine Lzip-Archivdatei dar. Verwenden Sie sie, um Lzip-Archive zu erstellen oder zu extrahieren.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [LzipArchive()](#LzipArchive--) | Initialisiert eine neue Instanz des [LzipArchive](../../com.aspose.zip/lziparchive). |
| [LzipArchive(LzipArchiveSettings settings)](#LzipArchive-com.aspose.zip.LzipArchiveSettings-) | Initialisiert eine neue Instanz des [LzipArchive](../../com.aspose.zip/lziparchive). |
| [LzipArchive(InputStream sourceStream)](#LzipArchive-java.io.InputStream-) | Initialisiert eine neue Instanz der [LzipArchive](../../com.aspose.zip/lziparchive)-Klasse, die für die Dekomprimierung vorbereitet ist. |
| [LzipArchive(InputStream sourceStream, LzipLoadOptions options)](#LzipArchive-java.io.InputStream-com.aspose.zip.LzipLoadOptions-) | Initialisiert eine neue Instanz der [LzipArchive](../../com.aspose.zip/lziparchive)-Klasse, die für die Dekomprimierung vorbereitet ist. |
| [LzipArchive(String path)](#LzipArchive-java.lang.String-) | Initialisiert eine neue Instanz der [LzipArchive](../../com.aspose.zip/lziparchive)-Klasse, die für die Dekomprimierung vorbereitet ist. |
| [LzipArchive(String path, LzipLoadOptions options)](#LzipArchive-java.lang.String-com.aspose.zip.LzipLoadOptions-) | Initialisiert eine neue Instanz der [LzipArchive](../../com.aspose.zip/lziparchive)-Klasse, die für die Dekomprimierung vorbereitet ist. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | Extrahiert das lzip-Archiv in eine Datei. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrahiert das lzip-Archiv in einen Stream. |
| [extract(String path)](#extract-java.lang.String-) | Extrahiert das lzip-Archiv in eine Datei über den Pfad. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrahiert den Inhalt des Archivs in das angegebene Verzeichnis. |
| [getFileEntries()](#getFileEntries--) | Liefert Einträge vom Typ [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), die das lzip-Archiv bilden. |
| [getFormat()](#getFormat--) | Liefert das Archivformat. |
| [getLength()](#getLength--) | Liefert die Länge. |
| [getName()](#getName--) | Der Name der Originaldatei. |
| [getSettings()](#getSettings--) | Liefert die Einstellung eines bestimmten lzip-Archivs. |
| [getUncompressedSize()](#getUncompressedSize--) | Liefert die unkomprimierte Größe der Dateidaten in Bytes. |
| [save(File destination)](#save-java.io.File-) | Speichert das lzip-Archiv in die angegebene Zieldatei. |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | Speichert das lzip-Archiv in den angegebenen Stream. |
| [save(String destinationFileName)](#save-java.lang.String-) | Speichert das lzip-Archiv in die angegebene Zieldatei. |
| [setSource(File file)](#setSource-java.io.File-) | Legt den Inhalt fest, der im Archiv komprimiert werden soll. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Legt den Inhalt fest, der im Archiv komprimiert werden soll. |
| [setSource(String path)](#setSource-java.lang.String-) | Legt den Inhalt fest, der im Archiv komprimiert werden soll. |
### LzipArchive() {#LzipArchive--}
```
public LzipArchive()
```


Initialisiert eine neue Instanz des [LzipArchive](../../com.aspose.zip/lziparchive).

### LzipArchive(LzipArchiveSettings settings) {#LzipArchive-com.aspose.zip.LzipArchiveSettings-}
```
public LzipArchive(LzipArchiveSettings settings)
```


Initialisiert eine neue Instanz des [LzipArchive](../../com.aspose.zip/lziparchive).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| settings | [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) | die Einstellung eines bestimmten lzip-Archivs mit Definition der Wörterbuchgröße |

### LzipArchive(InputStream sourceStream) {#LzipArchive-java.io.InputStream-}
```
public LzipArchive(InputStream sourceStream)
```


Initialisiert eine neue Instanz der [LzipArchive](../../com.aspose.zip/lziparchive)-Klasse, die für die Dekomprimierung vorbereitet ist.

```

``````

try (FileInputStream sourceLzipFile = new FileInputStream("sourceLzipFile")) {
try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
try (LzipArchive archive = new LzipArchive(sourceLzipFile)) {
archive.extract(extractedFile);
}
}
} catch (IOException ex) {
}
 
```

This constructor does not decompress. See [extract(OutputStream)](../../com.aspose.zip/lziparchive\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |

### LzipArchive(InputStream sourceStream, LzipLoadOptions options) {#LzipArchive-java.io.InputStream-com.aspose.zip.LzipLoadOptions-}
```
public LzipArchive(InputStream sourceStream, LzipLoadOptions options)
```


Initializes a new instance of the [LzipArchive](../../com.aspose.zip/lziparchive) class prepared for decompressing.

```

``````

     try (FileInputStream sourceLzipFile = new FileInputStream("sourceLzipFile")) {
         try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
             try (LzipArchive archive = new LzipArchive(sourceLzipFile)) {
                 archive.extract(extractedFile);
             }
         }
     } catch (IOException ex) {
     }
 
```

Dieser Konstruktor dekomprimiert nicht. Siehe die Methode [extract(OutputStream)](../../com.aspose.zip/lziparchive\#extract-OutputStream-) zum Dekomprimieren.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceStream | java.io.InputStream | die Quelle des Archivs |
| options | [LzipLoadOptions](../../com.aspose.zip/lziploadoptions) | Optionen zum Laden des Archivs. |

### LzipArchive(String path) {#LzipArchive-java.lang.String-}
```
public LzipArchive(String path)
```


Initialisiert eine neue Instanz der [LzipArchive](../../com.aspose.zip/lziparchive)-Klasse, die für die Dekomprimierung vorbereitet ist.

```

``````

try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
try (LzipArchive archive = new LzipArchive("sourceLzipFileName")) {
archive.extract(extractedFile);
}
} catch (IOException ex) {
}
 
```

This constructor does not decompress. See [extract(OutputStream)](../../com.aspose.zip/lziparchive\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the source of the archive |

### LzipArchive(String path, LzipLoadOptions options) {#LzipArchive-java.lang.String-com.aspose.zip.LzipLoadOptions-}
```
public LzipArchive(String path, LzipLoadOptions options)
```


Initializes a new instance of the [LzipArchive](../../com.aspose.zip/lziparchive) class prepared for decompressing.

```

``````

     try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
         try (LzipArchive archive = new LzipArchive("sourceLzipFileName")) {
             archive.extract(extractedFile);
         }
     } catch (IOException ex) {
     }
 
```

Dieser Konstruktor dekomprimiert nicht. Siehe die Methode [extract(OutputStream)](../../com.aspose.zip/lziparchive\#extract-OutputStream-) zum Dekomprimieren.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | java.lang.String | der Pfad zur Quelle des Archivs |
| options | [LzipLoadOptions](../../com.aspose.zip/lziploadoptions) | Optionen zum Laden des Archivs. |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Extrahiert das lzip-Archiv in eine Datei.

```

``````

try (FileInputStream lzipFile = new FileInputStream("sourceFileName")) {
try (LzipArchive archive = new LzipArchive(lzipFile)) {
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


Extracts lzip archive to a stream.

```

``````

     try (FileInputStream sourceLzipFile = new FileInputStream("sourceLzipFile")) {
         try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
             try (LzipArchive archive = new LzipArchive(sourceLzipFile)) {
                 archive.extract(extractedFile);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Ziel | java.io.OutputStream | der Stream zum Speichern der dekomprimierten Daten |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extrahiert das lzip-Archiv in eine Datei über den Pfad.

```

``````

try (FileInputStream lzipFile = new FileInputStream("sourceFileName")) {
try (LzipArchive archive = new LzipArchive(lzipFile)) {
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
java.io.File - the file info of the extracted file
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


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the lzip archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the lzip archive
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
java.lang.Long - length
### getName() {#getName--}
```
public final String getName()
```


The name of original file.

**Returns:**
java.lang.String - the name of the original file
### getSettings() {#getSettings--}
```
public final LzipArchiveSettings getSettings()
```


Gets the setting of particular lzip archive.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the setting of particular lzip archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets the uncompressed size of the file data in bytes.

**Returns:**
long - the uncompressed size of the file data in bytes
### save(File destination) {#save-java.io.File-}
```
public final void save(File destination)
```


Saves lzip archive to destination file provided.

```

``````

     try (LzipArchive archive = new LzipArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(new File("archive.lz"));
     }
 
```



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Ziel | java.io.File | die Datei, die als Ziel-Stream geöffnet wird |

### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


Speichert das lzip-Archiv in den angegebenen Stream.

```

``````

try (FileOutputStream lzFile = new FileOutputStream("archive.lz")) {
try (LzipArchive archive = new LzipArchive()) {
archive.setSource("data.bin");
archive.save(lzFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outputStream | java.io.OutputStream | destination stream |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves lzip archive to destination file provided.

```

``````

     try (LzipArchive archive = new LzipArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("result.lz");
     }
 
```



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| destinationFileName | java.lang.String | der Pfad des zu erstellenden Archivs. Wenn der angegebene Dateiname auf eine bereits vorhandene Datei verweist, wird sie überschrieben |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Legt den Inhalt fest, der im Archiv komprimiert werden soll.

```

``````

try (LzipArchive archive = new LzipArchive()) {
archive.setSource(new File("data.bin"));
archive.save("archive.lz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | the file which will be opened as input stream |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Sets the content to be compressed within the archive.

```

``````

     try (LzipArchive archive = new LzipArchive()) {
         archive.setSource(new ByteArrayInputStream(new byte[] {0x00, (byte)0xFF} ));
         archive.save("archive.lz");
     }
 
```



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| source | java.io.InputStream | der Eingabestream für das Archiv |

### setSource(String path) {#setSource-java.lang.String-}
```
public final void setSource(String path)
```


Legt den Inhalt fest, der im Archiv komprimiert werden soll.

```

``````

try (LzipArchive archive = new LzipArchive()) {
archive.setSource("data.bin");
archive.save("archive.lz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the file to be compressed |

