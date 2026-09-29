---
title: "LzmaArchive"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Diese Klasse stellt eine LZMA-Archivdatei dar."
type: docs
weight: 86
url: /de/java/com.aspose.zip/lzmaarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class LzmaArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

Diese Klasse repräsentiert eine LZMA-Archivdatei. Verwenden Sie sie, um LZMA-Archive zu erstellen oder zu extrahieren.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [LzmaArchive()](#LzmaArchive--) | Initialisiert eine neue Instanz der Klasse [LzmaArchive](../../com.aspose.zip/lzmaarchive) und erstellt das Archiv im LZMA-Format. |
| [LzmaArchive(LzmaArchiveSettings settings)](#LzmaArchive-com.aspose.zip.LzmaArchiveSettings-) | Initialisiert eine neue Instanz der Klasse [LzmaArchive](../../com.aspose.zip/lzmaarchive) und erstellt das Archiv im LZMA-Format. |
| [LzmaArchive(InputStream source)](#LzmaArchive-java.io.InputStream-) | Initialisiert eine neue Instanz der Klasse [LzmaArchive](../../com.aspose.zip/lzmaarchive), die für die Dekomprimierung vorbereitet ist. |
| [LzmaArchive(String path)](#LzmaArchive-java.lang.String-) | Initialisiert eine neue Instanz der Klasse [LzmaArchive](../../com.aspose.zip/lzmaarchive), die für die Dekomprimierung vorbereitet ist. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | Extrahiert das LZMA-Archiv in eine Datei. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrahiert das LZMA-Archiv in einen Stream. |
| [extract(String path)](#extract-java.lang.String-) | Extrahiert das LZMA-Archiv in eine Datei anhand des Pfads. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrahiert den Inhalt des Archivs in das angegebene Verzeichnis. |
| [getFileEntries()](#getFileEntries--) | Ermittelt Einträge vom Typ [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), die das LZMA-Archiv bilden. |
| [getFormat()](#getFormat--) | Liefert das Archivformat. |
| [getLength()](#getLength--) | Liefert die Länge. |
| [getName()](#getName--) | Der Name der Originaldatei. |
| [save(File destination)](#save-java.io.File-) | Speichert das LZMA-Archiv in die angegebene Zieldatei. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Speichert das lzma-Archiv in den bereitgestellten Stream. |
| [save(String destinationFileName)](#save-java.lang.String-) | Speichert das LZMA-Archiv in die angegebene Zieldatei. |
| [setSource(File file)](#setSource-java.io.File-) | Legt den Inhalt fest, der im Archiv komprimiert werden soll. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Legt den Inhalt fest, der im Archiv komprimiert werden soll. |
| [setSource(String sourcePath)](#setSource-java.lang.String-) | Legt den Inhalt fest, der im Archiv komprimiert werden soll. |
### LzmaArchive() {#LzmaArchive--}
```
public LzmaArchive()
```


Initialisiert eine neue Instanz der Klasse [LzmaArchive](../../com.aspose.zip/lzmaarchive) und erstellt das Archiv im LZMA-Format.

### LzmaArchive(LzmaArchiveSettings settings) {#LzmaArchive-com.aspose.zip.LzmaArchiveSettings-}
```
public LzmaArchive(LzmaArchiveSettings settings)
```


Initialisiert eine neue Instanz der Klasse [LzmaArchive](../../com.aspose.zip/lzmaarchive) und erstellt das Archiv im LZMA-Format.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| settings | [LzmaArchiveSettings](../../com.aspose.zip/lzmaarchivesettings) | Satz von Einstellungen für ein bestimmtes lzma-Archiv |

### LzmaArchive(InputStream source) {#LzmaArchive-java.io.InputStream-}
```
public LzmaArchive(InputStream source)
```


Initialisiert eine neue Instanz der Klasse [LzmaArchive](../../com.aspose.zip/lzmaarchive), die für die Dekomprimierung vorbereitet ist.

Dieser Konstruktor dekomprimiert nicht. Siehe die Methode [extract(OutputStream)](../../com.aspose.zip/lzmaarchive\#extract-OutputStream-) zum Dekomprimieren.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| source | java.io.InputStream | die Quelle des Archivs |

### LzmaArchive(String path) {#LzmaArchive-java.lang.String-}
```
public LzmaArchive(String path)
```


Initialisiert eine neue Instanz der Klasse [LzmaArchive](../../com.aspose.zip/lzmaarchive), die für die Dekomprimierung vorbereitet ist.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Datei | java.io.File | die Datei zum Speichern der dekomprimierten Daten |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extrahiert das LZMA-Archiv in einen Stream.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | java.lang.String | Der Pfad zu der Datei, die die dekomprimierten Daten speichert. |

**Returns:**
java.io.File - die Dateiinformation der extrahierten Datei
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extrahiert den Inhalt des Archivs in das angegebene Verzeichnis.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | destinationDirectory | java.lang.String | der Pfad zu dem Verzeichnis, in das die extrahierten Dateien abgelegt werden sollen. |

Wenn das Verzeichnis nicht existiert, wird es erstellt |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Ermittelt Einträge vom Typ [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), die das LZMA-Archiv bilden.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - Einträge des Typs [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), die das lzma-Archiv bilden.
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Liefert das Archivformat.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getLength() {#getLength--}
```
public final Long getLength()
```


Liefert die Länge.

**Returns:**
java.lang.Long - Länge
### getName() {#getName--}
```
public final String getName()
```


Der Name der Originaldatei.

**Returns:**
java.lang.String - der Name der Originaldatei
### save(File destination) {#save-java.io.File-}
```
public final void save(File destination)
```


Speichert das LZMA-Archiv in die angegebene Zieldatei.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Ausgabe | java.io.OutputStream | Ziel-Stream |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Speichert das LZMA-Archiv in die angegebene Zieldatei.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Datei | java.io.File | die Datei, die als Eingabestream geöffnet wird |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Legt den Inhalt fest, der im Archiv komprimiert werden soll.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourcePath | java.lang.String | Pfad zur Datei, die als Eingabestream geöffnet wird |

