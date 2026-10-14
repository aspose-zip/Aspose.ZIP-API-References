---
title: "IsoArchive"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Stellt ein ISO-Archiv nach ISO 9660 dar."
type: docs
weight: 71
url: /de/java/com.aspose.zip/isoarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public final class IsoArchive implements IArchive, AutoCloseable
```

Stellt ein ISO-Archiv (ISO 9660) dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [IsoArchive()](#IsoArchive--) | Initialisiert eine neue Instanz der Klasse [IsoArchive](../../com.aspose.zip/isoarchive) und erstellt ein leeres ISO-Archiv zum Hinzufügen neuer Dateien und Verzeichnisse. |
| [IsoArchive(InputStream sourceStream)](#IsoArchive-java.io.InputStream-) | Initialisiert eine neue Instanz der Klasse [IsoArchive](../../com.aspose.zip/isoarchive) und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann. |
| [IsoArchive(InputStream sourceStream, IsoLoadOptions loadOptions)](#IsoArchive-java.io.InputStream-com.aspose.zip.IsoLoadOptions-) | Initialisiert eine neue Instanz der Klasse [IsoArchive](../../com.aspose.zip/isoarchive) und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann. |
| [IsoArchive(String path)](#IsoArchive-java.lang.String-) | Initialisiert eine neue Instanz der Klasse [IsoArchive](../../com.aspose.zip/isoarchive) und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann. |
| [IsoArchive(String path, IsoLoadOptions loadOptions)](#IsoArchive-java.lang.String-com.aspose.zip.IsoLoadOptions-) | Initialisiert eine neue Instanz der Klasse [IsoArchive](../../com.aspose.zip/isoarchive) und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createDirectory(String name)](#createDirectory-java.lang.String-) | Fügt dem ISO-Image ein Verzeichnis hinzu. |
| [createEntry(String name)](#createEntry-java.lang.String-) | Fügt dem ISO-Image eine Datei hinzu. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | Fügt dem ISO-Image eine Datei hinzu. |
| [createEntry(String name, String filePath)](#createEntry-java.lang.String-java.lang.String-) | Fügt dem ISO-Image eine Datei hinzu. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrahiert alle Einträge in das angegebene Verzeichnis. |
| [getEntries()](#getEntries--) | Ruft Einträge vom Typ [IsoEntry](../../com.aspose.zip/isoentry) ab, die das Archiv bilden. |
| [getFileEntries()](#getFileEntries--) | Ruft Einträge vom Typ [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) ab, die das Archiv bilden. |
| [getFormat()](#getFormat--) | Liefert das Archivformat. |
| [save(OutputStream stream)](#save-java.io.OutputStream-) | Speichert das ISO-Image in den angegebenen Stream. |
| [save(OutputStream stream, IsoSaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.IsoSaveOptions-) | Speichert das ISO-Image in den angegebenen Stream. |
| [save(String path)](#save-java.lang.String-) | Speichert das ISO-Image im angegebenen Pfad. |
| [save(String path, IsoSaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.IsoSaveOptions-) | Speichert das ISO-Image im angegebenen Pfad. |
### IsoArchive() {#IsoArchive--}
```
public IsoArchive()
```


Initialisiert eine neue Instanz der Klasse [IsoArchive](../../com.aspose.zip/isoarchive) und erstellt ein leeres ISO-Archiv zum Hinzufügen neuer Dateien und Verzeichnisse.

Das folgende Beispiel zeigt, wie man ein neues leeres ISO-Archiv erstellt und Dateien hinzufügt:

```

``````

// Erstelle ein neues leeres ISO-Archiv
try (IsoArchive isoArchive = new IsoArchive()) {
// Dateien zum ISO-Archiv hinzufügen
isoArchive.createEntry("example_file.txt", "path_to_file.txt");
// Speichere das ISO-Archiv in einer Datei
isoArchive.save("new_archive.iso");
}
 
```



### IsoArchive(InputStream sourceStream) {#IsoArchive-java.io.InputStream-}
```
public IsoArchive(InputStream sourceStream)
```


Initializes a new instance of the [IsoArchive](../../com.aspose.zip/isoarchive) class and composes an entry list that can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (IsoArchive archive = new IsoArchive(new FileInputStream("archive.iso"))) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

Dieser Konstruktor entpackt keinen Eintrag.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceStream | java.io.InputStream | die Quelle des Archivs |

### IsoArchive(InputStream sourceStream, IsoLoadOptions loadOptions) {#IsoArchive-java.io.InputStream-com.aspose.zip.IsoLoadOptions-}
```
public IsoArchive(InputStream sourceStream, IsoLoadOptions loadOptions)
```


Initialisiert eine neue Instanz der Klasse [IsoArchive](../../com.aspose.zip/isoarchive) und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann.

Das folgende Beispiel zeigt, wie man alle Einträge in ein Verzeichnis extrahiert.

```

``````

try (IsoArchive archive = new IsoArchive(new FileInputStream("archive.iso"))) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |
| loadOptions | [IsoLoadOptions](../../com.aspose.zip/isoloadoptions) | the options to load archive with |

### IsoArchive(String path) {#IsoArchive-java.lang.String-}
```
public IsoArchive(String path)
```


Initializes a new instance of the [IsoArchive](../../com.aspose.zip/isoarchive) class and composes an entry list that can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (IsoArchive archive = new IsoArchive("archive.iso")) {
         archive.extractToDirectory("C:\\extracted");
     }
 
```

Dieser Konstruktor entpackt keinen Eintrag.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | java.lang.String | der Pfad zur Archivdatei |

### IsoArchive(String path, IsoLoadOptions loadOptions) {#IsoArchive-java.lang.String-com.aspose.zip.IsoLoadOptions-}
```
public IsoArchive(String path, IsoLoadOptions loadOptions)
```


Initialisiert eine neue Instanz der Klasse [IsoArchive](../../com.aspose.zip/isoarchive) und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann.

Das folgende Beispiel zeigt, wie man alle Einträge in ein Verzeichnis extrahiert.

```

``````

try (IsoArchive archive = new IsoArchive("archive.iso")) {
archive.extractToDirectory("C:\\extracted");
}
 
```

This constructor does not unpack any entry.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |
| loadOptions | [IsoLoadOptions](../../com.aspose.zip/isoloadoptions) | the options to load archive with |

### close() {#close--}
```
public void close()
```




### createDirectory(String name) {#createDirectory-java.lang.String-}
```
public final IsoEntry createDirectory(String name)
```


Adds a directory to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the directory in the ISO |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### createEntry(String name) {#createEntry-java.lang.String-}
```
public final IsoEntry createEntry(String name)
```


Adds a file to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the file in the ISO |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final IsoEntry createEntry(String name, InputStream source)
```


Adds a file to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the file in the ISO |
| source | java.io.InputStream | the stream containing the file data |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### createEntry(String name, String filePath) {#createEntry-java.lang.String-java.lang.String-}
```
public final IsoEntry createEntry(String name, String filePath)
```


Adds a file to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the file in the ISO |
| filePath | java.lang.String | the path of the file |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all entries to the specified directory.

The following example shows how to extract all entries to a directory:

```

``````

     try (IsoArchive archive = new IsoArchive(new FileInputStream("archive.iso"))) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| destinationDirectory | java.lang.String | das Verzeichnis, in das die Einträge extrahiert werden sollen |

### getEntries() {#getEntries--}
```
public final List<IsoEntry> getEntries()
```


Ruft Einträge vom Typ [IsoEntry](../../com.aspose.zip/isoentry) ab, die das Archiv bilden.

**Returns:**
java.util.List&lt;com.aspose.zip.IsoEntry&gt; - Einträge des Typs [IsoEntry](../../com.aspose.zip/isoentry), die das ISO-Archiv bilden
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Ruft Einträge vom Typ [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) ab, die das Archiv bilden.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - Einträge des Typs [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), die das ISO-Archiv bilden
### getFormat() {#getFormat--}
```
public ArchiveFormat getFormat()
```


Liefert das Archivformat.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream stream)
```


Speichert das ISO-Image in den angegebenen Stream.

Das folgende Beispiel zeigt, wie ein ISO-Archiv in einen Speicherstrom gespeichert wird:

```

``````

ByteArrayOutputStream memoryStream = new ByteArrayOutputStream();
// Erstelle ein neues leeres ISO-Archiv
try (IsoArchive isoArchive = new IsoArchive()) {
// Dateien zum ISO-Archiv hinzufügen
isoArchive.createEntry("example_file.txt", "path_to_file.txt");
// Speichert das ISO-Archiv in einen Speicherstrom
isoArchive.save(memoryStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | the stream where the ISO image will be saved |

### save(OutputStream stream, IsoSaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.IsoSaveOptions-}
```
public final void save(OutputStream stream, IsoSaveOptions saveOptions)
```


Saves the ISO image to the specified stream.

The following example shows how to save an ISO archive to a memory stream:

```

``````

     ByteArrayOutputStream memoryStream = new ByteArrayOutputStream();
     // Create a new empty ISO archive
     try (IsoArchive isoArchive = new IsoArchive()) {
         // Add files to the ISO archive
         isoArchive.createEntry("example_file.txt", "path_to_file.txt");
         // Save the ISO archive to a memory stream
         isoArchive.save(memoryStream);
     }
 
```



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stream | java.io.OutputStream | der Stream, in dem das ISO-Image gespeichert wird |
| saveOptions | [IsoSaveOptions](../../com.aspose.zip/isosaveoptions) | die Optionen, mit denen das ISO-Archiv gespeichert wird |

### save(String path) {#save-java.lang.String-}
```
public final void save(String path)
```


Speichert das ISO-Image im angegebenen Pfad.

Das folgende Beispiel zeigt, wie ein ISO-Archiv in einer Datei gespeichert wird:

```

``````

// Erstelle ein neues leeres ISO-Archiv
try (IsoArchive isoArchive = new IsoArchive()) {
// Dateien zum ISO-Archiv hinzufügen
isoArchive.createEntry("example_file.txt", "path_to_file.txt");
// Speichere das ISO-Archiv in einer Datei
isoArchive.save("new_archive.iso");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path where the ISO image will be saved |

### save(String path, IsoSaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.IsoSaveOptions-}
```
public final void save(String path, IsoSaveOptions saveOptions)
```


Saves the ISO image to the specified path.

The following example shows how to save an ISO archive to a file:

```

``````

     // Create a new empty ISO archive
     try (IsoArchive isoArchive = new IsoArchive()) {
         // Add files to the ISO archive
         isoArchive.createEntry("example_file.txt", "path_to_file.txt");
         // Save the ISO archive to a file
         isoArchive.save("new_archive.iso");
     }
 
```



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | java.lang.String | der Pfad, an dem das ISO-Image gespeichert wird |
| saveOptions | [IsoSaveOptions](../../com.aspose.zip/isosaveoptions) | die Optionen, mit denen das ISO-Archiv gespeichert wird |

