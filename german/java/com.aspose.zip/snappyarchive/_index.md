---
title: "SnappyArchive"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Diese Klasse repräsentiert eine Snappy-Archivdatei."
type: docs
weight: 121
url: /de/java/com.aspose.zip/snappyarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class SnappyArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

Diese Klasse repräsentiert eine Snappy-Archivdatei. Verwenden Sie sie, um Snappy-Archive zu erstellen oder zu extrahieren.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [SnappyArchive()](#SnappyArchive--) | Initialisiert eine neue Instanz der [SnappyArchive](../../com.aspose.zip/snappyarchive)-Klasse, die zum Komprimieren vorbereitet ist. |
| [SnappyArchive(InputStream source)](#SnappyArchive-java.io.InputStream-) | Initialisiert eine neue Instanz der [SnappyArchive](../../com.aspose.zip/snappyarchive)-Klasse, die zum Dekomprimieren vorbereitet ist. |
| [SnappyArchive(String path)](#SnappyArchive-java.lang.String-) | Initialisiert eine neue Instanz der [SnappyArchive](../../com.aspose.zip/snappyarchive)-Klasse, die zum Dekomprimieren vorbereitet ist. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | Extrahiert das Snappy-Archiv in eine Datei. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrahiert das Snappy-Archiv in einen Stream. |
| [extract(String path)](#extract-java.lang.String-) | Extrahiert das Snappy-Archiv in eine Datei über den Pfad. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrahiert den Inhalt des Archivs in das angegebene Verzeichnis. |
| [getFileEntries()](#getFileEntries--) | Gibt Einträge vom Typ [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) zurück, die das Snappy-Archiv bilden. |
| [getFormat()](#getFormat--) | Liefert das Archivformat. |
| [getLength()](#getLength--) | Liefert die Länge. |
| [getName()](#getName--) | Der Name der Originaldatei. |
| [save(File destination)](#save-java.io.File-) | Speichert das Snappy-Archiv in die angegebene Zieldatei. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Speichert das Snappy-Archiv in den angegebenen Stream. |
| [save(String destinationFileName)](#save-java.lang.String-) | Speichert das Snappy-Archiv in die angegebene Zieldatei. |
| [setSource(File file)](#setSource-java.io.File-) | Legt den Inhalt fest, der im Archiv komprimiert werden soll. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Legt den Inhalt fest, der im Archiv komprimiert werden soll. |
| [setSource(String sourcePath)](#setSource-java.lang.String-) | Legt den Inhalt fest, der im Archiv komprimiert werden soll. |
### SnappyArchive() {#SnappyArchive--}
```
public SnappyArchive()
```


Initialisiert eine neue Instanz der [SnappyArchive](../../com.aspose.zip/snappyarchive)-Klasse, die zum Komprimieren vorbereitet ist.

Das folgende Beispiel zeigt, wie man eine Datei komprimiert.

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

Dieser Konstruktor dekomprimiert nicht. Siehe die Methode [extract(java.io.OutputStream)](../../com.aspose.zip/snappyarchive\#extract-java.io.OutputStream-) zum Dekomprimieren.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | java.lang.String | der Pfad zur Quelle des Archivs |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Extrahiert das Snappy-Archiv in eine Datei.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Ziel | java.io.OutputStream | der Stream zum Speichern der dekomprimierten Daten |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extrahiert das Snappy-Archiv in eine Datei über den Pfad.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Ziel | java.io.File | die Datei, die als Ziel-Stream geöffnet wird |

### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Speichert das Snappy-Archiv in den angegebenen Stream.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| source | java.io.InputStream | der Eingabestream für das Archiv |

### setSource(String sourcePath) {#setSource-java.lang.String-}
```
public final void setSource(String sourcePath)
```


Legt den Inhalt fest, der im Archiv komprimiert werden soll.

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

