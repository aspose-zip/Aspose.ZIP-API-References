---
title: "XzArchive"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Diese Klasse stellt eine xz-Archivdatei dar."
type: docs
weight: 146
url: /de/java/com.aspose.zip/xzarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), [com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class XzArchive implements IArchiveFileEntry, IArchive, AutoCloseable
```

Diese Klasse repräsentiert eine xz-Archivdatei. Verwenden Sie sie, um xz-Archive zu erstellen und zu extrahieren.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [XzArchive()](#XzArchive--) | Initialisiert eine neue Instanz der Klasse [XzArchive](../../com.aspose.zip/xzarchive) und erstellt das Archiv im xz-Format. |
| [XzArchive(XzArchiveSettings settings)](#XzArchive-com.aspose.zip.XzArchiveSettings-) | Initialisiert eine neue Instanz der Klasse [XzArchive](../../com.aspose.zip/xzarchive) und erstellt das Archiv im xz-Format. |
| [XzArchive(InputStream source)](#XzArchive-java.io.InputStream-) | Initialisiert eine neue Instanz der Klasse [XzArchive](../../com.aspose.zip/xzarchive), die zum Dekomprimieren vorbereitet ist. |
| [XzArchive(InputStream source, XzLoadOptions options)](#XzArchive-java.io.InputStream-com.aspose.zip.XzLoadOptions-) | Initialisiert eine neue Instanz der Klasse [XzArchive](../../com.aspose.zip/xzarchive), die zum Dekomprimieren vorbereitet ist. |
| [XzArchive(String path)](#XzArchive-java.lang.String-) | Initialisiert eine neue Instanz der Klasse [XzArchive](../../com.aspose.zip/xzarchive), die zum Dekomprimieren vorbereitet ist. |
| [XzArchive(String path, XzLoadOptions options)](#XzArchive-java.lang.String-com.aspose.zip.XzLoadOptions-) | Initialisiert eine neue Instanz der Klasse [XzArchive](../../com.aspose.zip/xzarchive), die zum Dekomprimieren vorbereitet ist. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | Extrahiert ein xz-Archiv in eine Datei. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrahiert ein xz-Archiv in einen Stream. |
| [extract(String path)](#extract-java.lang.String-) | Extrahiert ein xz-Archiv in eine Datei anhand des Pfads. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrahiert den Inhalt des Archivs in das angegebene Verzeichnis. |
| [getFileEntries()](#getFileEntries--) | Liefert Einträge des Typs [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), die das xz-Archiv bilden. |
| [getFormat()](#getFormat--) | Liefert das Archivformat. |
| [getLength()](#getLength--) | Gibt die Länge des Eintrags in Bytes zurück. |
| [getName()](#getName--) | Liefert den Namen des Eintrags im Archiv. |
| [getUncompressedSize()](#getUncompressedSize--) | Liefert die unkomprimierte Größe der Dateidaten in Bytes. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Speichert das xz-Archiv in den bereitgestellten Stream. |
| [save(String destinationFileName)](#save-java.lang.String-) | Speichert das xz-Archiv in die angegebene Zieldatei. |
| [setSource(File file)](#setSource-java.io.File-) | Legt den Inhalt fest, der im Archiv komprimiert werden soll. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Legt den Inhalt fest, der im Archiv komprimiert werden soll. |
| [setSource(String sourcePath)](#setSource-java.lang.String-) | Legt den Inhalt fest, der im Archiv komprimiert werden soll. |
### XzArchive() {#XzArchive--}
```
public XzArchive()
```


Initialisiert eine neue Instanz der Klasse [XzArchive](../../com.aspose.zip/xzarchive) und erstellt das Archiv im xz-Format.

### XzArchive(XzArchiveSettings settings) {#XzArchive-com.aspose.zip.XzArchiveSettings-}
```
public XzArchive(XzArchiveSettings settings)
```


Initialisiert eine neue Instanz der Klasse [XzArchive](../../com.aspose.zip/xzarchive) und erstellt das Archiv im xz-Format.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| settings | [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) | Satz von Einstellungen für ein bestimmtes xz-Archiv: Wörterbuchgröße, Blockgröße, Prüftyp |

### XzArchive(InputStream source) {#XzArchive-java.io.InputStream-}
```
public XzArchive(InputStream source)
```


Initialisiert eine neue Instanz der Klasse [XzArchive](../../com.aspose.zip/xzarchive), die zum Dekomprimieren vorbereitet ist.

Dieser Konstruktor dekomprimiert nicht. Siehe die Methode [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\#extract-java.io.OutputStream-) zum Dekomprimieren.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| source | java.io.InputStream | die Quelle des Archivs |

### XzArchive(InputStream source, XzLoadOptions options) {#XzArchive-java.io.InputStream-com.aspose.zip.XzLoadOptions-}
```
public XzArchive(InputStream source, XzLoadOptions options)
```


Initialisiert eine neue Instanz der Klasse [XzArchive](../../com.aspose.zip/xzarchive), die zum Dekomprimieren vorbereitet ist.

Dieser Konstruktor dekomprimiert nicht. Siehe die Methode [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\#extract-java.io.OutputStream-) zum Dekomprimieren.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| source | java.io.InputStream | die Quelle des Archivs |
| options | [XzLoadOptions](../../com.aspose.zip/xzloadoptions) | Optionen zum Laden des Archivs. |

### XzArchive(String path) {#XzArchive-java.lang.String-}
```
public XzArchive(String path)
```


Initialisiert eine neue Instanz der Klasse [XzArchive](../../com.aspose.zip/xzarchive), die zum Dekomprimieren vorbereitet ist.

Dieser Konstruktor dekomprimiert nicht. Siehe die Methode [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\#extract-java.io.OutputStream-) zum Dekomprimieren.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | java.lang.String | Pfad zur Quelle des Archivs |

### XzArchive(String path, XzLoadOptions options) {#XzArchive-java.lang.String-com.aspose.zip.XzLoadOptions-}
```
public XzArchive(String path, XzLoadOptions options)
```


Initialisiert eine neue Instanz der Klasse [XzArchive](../../com.aspose.zip/xzarchive), die zum Dekomprimieren vorbereitet ist.

Dieser Konstruktor dekomprimiert nicht. Siehe die Methode [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\#extract-java.io.OutputStream-) zum Dekomprimieren.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | java.lang.String | Pfad zur Quelle des Archivs |
| options | [XzLoadOptions](../../com.aspose.zip/xzloadoptions) |  |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Extrahiert ein xz-Archiv in eine Datei.

```

``````

try (FileInputStream xzFile = new FileInputStream("sourceFileName")) {
try (XzArchive archive = new XzArchive(xzFile)) {
archive.extract(new File("extracted.bin"));
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | file for storing decompressed data |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts xz archive to a stream.

```

``````

     try (FileInputStream xzFile = new FileInputStream("sourceFileName")) {
         try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
             try (XzArchive archive = new XzArchive(xzFile)) {
                 archive.extract(extractedFile);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Ziel | java.io.OutputStream | Stream zum Speichern der dekomprimierten Daten |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extrahiert ein xz-Archiv in eine Datei anhand des Pfads.

```

``````

try (FileInputStream xzFile = new FileInputStream("sourceFileName")) {
try (XzArchive archive = new XzArchive(xzFile)) {
archive.extract("extracted.bin");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | path to file which will store decompressed data |

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

If the directory does not exist, it will be created. |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the xz archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the xz archive
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


Gets the length of the entry in bytes.

**Returns:**
java.lang.Long - the length of the entry in bytes
### getName() {#getName--}
```
public final String getName()
```


Gets the name of the entry within archive.

**Returns:**
java.lang.String - the name of the entry within archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets the uncompressed size of the file data in bytes.

**Returns:**
long - the uncompressed size of the file data in bytes
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves xz archive to the stream provided.

```

``````

     try (FileOutputStream xzFile = new FileOutputStream("archive.xz")) {
         try (XzArchive archive = new XzArchive()) {
             archive.setSource("data.bin");
             archive.save(xzFile);
         }
     } catch (IOException ex) {
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


Speichert das xz-Archiv in die angegebene Zieldatei.

```

``````

try (XzArchive archive = new XzArchive()) {
archive.setSource(new File("data.bin"));
archive.save("result.xz");
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

     try (XzArchive archive = new XzArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.xz");
     }
 
```



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Datei | java.io.File | Datei, die als Eingabestream geöffnet wird |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Legt den Inhalt fest, der im Archiv komprimiert werden soll.

```

``````

try (XzArchive archive = new XzArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] { 0x00, (byte) 0xFF }));
archive.save("archive.xz");
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

     try (XzArchive archive = new XzArchive()) {
         archive.setSource("data.bin");
         archive.save("archive.xz");
     }
 
```



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourcePath | java.lang.String | Pfad zur Datei, die als Eingabestream geöffnet wird |

