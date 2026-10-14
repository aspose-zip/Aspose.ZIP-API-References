---
title: "Archiv"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Diese Klasse stellt eine ZIP-Archivdatei dar."
type: docs
weight: 26
url: /de/java/com.aspose.zip/archive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class Archive implements IArchive, AutoCloseable
```

Diese Klasse stellt eine ZIP-Archivdatei dar. Verwenden Sie sie zum Erstellen, Extrahieren oder Aktualisieren von ZIP-Archiven.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [Archive()](#Archive--) | Initialisiert eine neue Instanz der [Archive](../../com.aspose.zip/archive)-Klasse mit optionalen Einstellungen für ihre Einträge. |
| [Archive(ArchiveEntrySettings newEntrySettings)](#Archive-com.aspose.zip.ArchiveEntrySettings-) | Initialisiert eine neue Instanz der [Archive](../../com.aspose.zip/archive)-Klasse mit optionalen Einstellungen für ihre Einträge. |
| [Archive(InputStream sourceStream)](#Archive-java.io.InputStream-) | Initialisiert eine neue Instanz der [Archive](../../com.aspose.zip/archive)-Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann. |
| [Archive(InputStream sourceStream, ArchiveLoadOptions loadOptions)](#Archive-java.io.InputStream-com.aspose.zip.ArchiveLoadOptions-) | Initialisiert eine neue Instanz der [Archive](../../com.aspose.zip/archive)-Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann. |
| [Archive(InputStream sourceStream, ArchiveLoadOptions loadOptions, ArchiveEntrySettings newEntrySettings)](#Archive-java.io.InputStream-com.aspose.zip.ArchiveLoadOptions-com.aspose.zip.ArchiveEntrySettings-) | Initialisiert eine neue Instanz der [Archive](../../com.aspose.zip/archive)-Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann. |
| [Archive(String path)](#Archive-java.lang.String-) | Initialisiert eine neue Instanz der [Archive](../../com.aspose.zip/archive)-Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann. |
| [Archive(String path, ArchiveLoadOptions loadOptions)](#Archive-java.lang.String-com.aspose.zip.ArchiveLoadOptions-) | Initialisiert eine neue Instanz der [Archive](../../com.aspose.zip/archive)-Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann. |
| [Archive(String path, ArchiveLoadOptions loadOptions, ArchiveEntrySettings newEntrySettings)](#Archive-java.lang.String-com.aspose.zip.ArchiveLoadOptions-com.aspose.zip.ArchiveEntrySettings-) | Initialisiert eine neue Instanz der [Archive](../../com.aspose.zip/archive)-Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann. |
| [Archive(String mainSegment, String[] segmentsInOrder)](#Archive-java.lang.String-java.lang.String---) | Initialisiert eine neue Instanz der [Archive](../../com.aspose.zip/archive)-Klasse aus einem mehrteiligen ZIP-Archiv und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann. |
| [Archive(String mainSegment, String[] segmentsInOrder, ArchiveLoadOptions loadOptions)](#Archive-java.lang.String-java.lang.String---com.aspose.zip.ArchiveLoadOptions-) | Initialisiert eine neue Instanz der [Archive](../../com.aspose.zip/archive)-Klasse aus einem mehrteiligen ZIP-Archiv und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | Fügt dem Archiv alle Dateien und Verzeichnisse rekursiv aus dem angegebenen Verzeichnis hinzu. |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | Fügt dem Archiv alle Dateien und Verzeichnisse rekursiv aus dem angegebenen Verzeichnis hinzu. |
| [createEntries(String sourceDirectory)](#createEntries-java.lang.String-) | Fügt dem Archiv alle Dateien und Verzeichnisse rekursiv aus dem angegebenen Verzeichnis hinzu. |
| [createEntries(String sourceDirectory, boolean includeRootDirectory)](#createEntries-java.lang.String-boolean-) | Fügt dem Archiv alle Dateien und Verzeichnisse rekursiv aus dem angegebenen Verzeichnis hinzu. |
| [createEntry(String name, File file)](#createEntry-java.lang.String-java.io.File-) | Erstellt einen einzelnen Eintrag im Archiv. |
| [createEntry(String name, File file, boolean openImmediately)](#createEntry-java.lang.String-java.io.File-boolean-) | Erstellt einen einzelnen Eintrag im Archiv. |
| [createEntry(String name, File file, boolean openImmediately, ArchiveEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.io.File-boolean-com.aspose.zip.ArchiveEntrySettings-) | Erstellt einen einzelnen Eintrag im Archiv. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | Erstellt einen einzelnen Eintrag im Archiv. |
| [createEntry(String name, InputStream source, ArchiveEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.ArchiveEntrySettings-) | Erstellt einen einzelnen Eintrag im Archiv. |
| [createEntry(String name, InputStream source, ArchiveEntrySettings newEntrySettings, File file)](#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.ArchiveEntrySettings-java.io.File-) | Erstellt einen einzelnen Eintrag im Archiv. |
| [createEntry(String name, String path)](#createEntry-java.lang.String-java.lang.String-) | Erstellt einen einzelnen Eintrag im Archiv. |
| [createEntry(String name, String path, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | Erstellt einen einzelnen Eintrag im Archiv. |
| [createEntry(String name, String path, boolean openImmediately, ArchiveEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.lang.String-boolean-com.aspose.zip.ArchiveEntrySettings-) | Erstellt einen einzelnen Eintrag im Archiv. |
| [createEntry(String name, Supplier&lt;InputStream&gt; streamProvider)](#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--) | Erstellt einen einzelnen Eintrag im Archiv. |
| [createEntry(String name, Supplier&lt;InputStream&gt; streamProvider, ArchiveEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--com.aspose.zip.ArchiveEntrySettings-) | Erstellt einen einzelnen Eintrag im Archiv. |
| [deleteEntry(ArchiveEntry entry)](#deleteEntry-com.aspose.zip.ArchiveEntry-) | Entfernt das erste Vorkommen des angegebenen Eintrags aus der Eintragsliste. |
| [deleteEntry(int entryIndex)](#deleteEntry-int-) | Entfernt den Eintrag aus der Eintragsliste anhand des Index. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrahiert alle Dateien im Archiv in das angegebene Verzeichnis. |
| [getComment()](#getComment--) | Liefert den Kommentar für das gesamte Archiv. |
| [getEntries()](#getEntries--) | Liefert Einträge vom Typ [ArchiveEntry](../../com.aspose.zip/archiveentry), die das Archiv bilden. |
| [getFileEntries()](#getFileEntries--) | Ruft Einträge vom Typ [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) ab, die das Archiv bilden. |
| [getFormat()](#getFormat--) | Liefert das Archivformat (Zip) |
| [getNewEntrySettings()](#getNewEntrySettings--) | Kompressions- und Verschlüsselungseinstellungen, die für neu hinzugefügte [ArchiveEntry](../../com.aspose.zip/archiveentry)-Elemente verwendet werden. |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | Speichert das Archiv in den angegebenen Stream. |
| [save(OutputStream outputStream, ArchiveSaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.ArchiveSaveOptions-) | Speichert das Archiv in den angegebenen Stream. |
| [save(String destinationFileName)](#save-java.lang.String-) | Speichert das Archiv in die angegebene Zieldatei. |
| [save(String destinationFileName, ArchiveSaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.ArchiveSaveOptions-) | Speichert das Archiv in die angegebene Zieldatei. |
| [saveSplit(String destinationDirectory, SplitArchiveSaveOptions options)](#saveSplit-java.lang.String-com.aspose.zip.SplitArchiveSaveOptions-) | Speichert ein mehrteiliges Archiv in das angegebene Zielverzeichnis. |
### Archive() {#Archive--}
```
public Archive()
```


Initialisiert eine neue Instanz der [Archive](../../com.aspose.zip/archive)-Klasse mit optionalen Einstellungen für ihre Einträge.


Das folgende Beispiel zeigt, wie man eine einzelne Datei mit den Standardeinstellungen komprimiert.

```

``````

try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
try (Archive archive = new Archive()) {
archive.createEntry("data.bin", "file.dat");
archive.save(zipFile);
}
} catch (IOException ex) {
}
 
```



### Archive(ArchiveEntrySettings newEntrySettings) {#Archive-com.aspose.zip.ArchiveEntrySettings-}
```
public Archive(ArchiveEntrySettings newEntrySettings)
```


Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class with optional settings for its entries.


The following example shows how to compress a single file with default settings.

```

``````

     try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
         try (Archive archive = new Archive()) {
             archive.createEntry("data.bin", "file.dat");
             archive.save(zipFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| newEntrySettings | [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) | Kompressions- und Verschlüsselungseinstellungen, die für neu hinzugefügte [ArchiveEntry](../../com.aspose.zip/archiveentry)-Elemente verwendet werden. Wenn nicht angegeben, wird die am häufigsten verwendete Deflate-Kompression ohne Verschlüsselung verwendet. |

### Archive(InputStream sourceStream) {#Archive-java.io.InputStream-}
```
public Archive(InputStream sourceStream)
```


Initialisiert eine neue Instanz der [Archive](../../com.aspose.zip/archive)-Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann.

Das folgende Beispiel extrahiert ein verschlüsseltes Archiv und dekomprimiert dann den ersten Eintrag in einen `ByteArrayOutputStream`.

```

``````

try (FileInputStream fs = new FileInputStream("encrypted.zip")) {
ByteArrayOutputStream extracted = new ByteArrayOutputStream();
ArchiveLoadOptions options = new ArchiveLoadOptions();
options.setDecryptionPassword("p@s$");
try (Archive archive = new Archive(fs, options)) {
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

This constructor does not decompress any entry. See [ArchiveEntry.open()](../../com.aspose.zip/archiveentry\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | The source of the archive. |

### Archive(InputStream sourceStream, ArchiveLoadOptions loadOptions) {#Archive-java.io.InputStream-com.aspose.zip.ArchiveLoadOptions-}
```
public Archive(InputStream sourceStream, ArchiveLoadOptions loadOptions)
```


Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class and composes an entry list can be extracted from the archive.

The following example extracts an encrypted archive, then decompresses first entry to a `ByteArrayOutputStream`.

```

``````

     try (FileInputStream fs = new FileInputStream("encrypted.zip")) {
         ByteArrayOutputStream extracted = new ByteArrayOutputStream();
         ArchiveLoadOptions options = new ArchiveLoadOptions();
         options.setDecryptionPassword("p@s$");
         try (Archive archive = new Archive(fs, options)) {
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

Dieser Konstruktor dekomprimiert keinen Eintrag. Siehe die Methode [ArchiveEntry.open()](../../com.aspose.zip/archiveentry\\#open--) zum Dekomprimieren.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceStream | java.io.InputStream | Die Quelle des Archivs. |
| loadOptions | [ArchiveLoadOptions](../../com.aspose.zip/archiveloadoptions) | Optionen zum Laden eines bestehenden Archivs. |

### Archive(InputStream sourceStream, ArchiveLoadOptions loadOptions, ArchiveEntrySettings newEntrySettings) {#Archive-java.io.InputStream-com.aspose.zip.ArchiveLoadOptions-com.aspose.zip.ArchiveEntrySettings-}
```
public Archive(InputStream sourceStream, ArchiveLoadOptions loadOptions, ArchiveEntrySettings newEntrySettings)
```


Initialisiert eine neue Instanz der [Archive](../../com.aspose.zip/archive)-Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann.

Das folgende Beispiel extrahiert ein verschlüsseltes Archiv und dekomprimiert dann den ersten Eintrag in einen `ByteArrayOutputStream`.

```

``````

try (FileInputStream fs = new FileInputStream("encrypted.zip")) {
ByteArrayOutputStream extracted = new ByteArrayOutputStream();
ArchiveLoadOptions options = new ArchiveLoadOptions();
options.setDecryptionPassword("p@s$");
try (Archive archive = new Archive(fs, options)) {
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

This constructor does not decompress any entry. See [ArchiveEntry.open()](../../com.aspose.zip/archiveentry\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | The source of the archive. |
| loadOptions | [ArchiveLoadOptions](../../com.aspose.zip/archiveloadoptions) | Options to load existing archive with. |
| newEntrySettings | [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) | Compression and encryption settings used for newly added [ArchiveEntry](../../com.aspose.zip/archiveentry) items. If not specified, the most common Deflate compression without encryption would be used. |

### Archive(String path) {#Archive-java.lang.String-}
```
public Archive(String path)
```


Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class and composes an entry list can be extracted from the archive.

The following example extracts an encrypted archive, then decompresses first entry to a `ByteArrayOutputStream`.

```

``````

     ByteArrayOutputStream extracted = new ByteArrayOutputStream();
     ArchiveLoadOptions options = new ArchiveLoadOptions();
     options.setDecryptionPassword("p@s$");
     try (Archive archive = new Archive("encrypted.zip", options)) {
         try (InputStream decompressed = archive.getEntries().get(0).open()) {
             byte[] b = new byte[8192];
             int bytesRead;
             while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
                 extracted.write(b, 0, bytesRead);
         } catch (IOException ex) {
         }
     }
 
```

Dieser Konstruktor dekomprimiert keinen Eintrag. Siehe die Methode [ArchiveEntry.open()](../../com.aspose.zip/archiveentry\\#open--) zum Dekomprimieren.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | java.lang.String | Der vollqualifizierte oder relative Pfad zur Archivdatei. |

### Archive(String path, ArchiveLoadOptions loadOptions) {#Archive-java.lang.String-com.aspose.zip.ArchiveLoadOptions-}
```
public Archive(String path, ArchiveLoadOptions loadOptions)
```


Initialisiert eine neue Instanz der [Archive](../../com.aspose.zip/archive)-Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann.

Das folgende Beispiel extrahiert ein verschlüsseltes Archiv und dekomprimiert dann den ersten Eintrag in einen `ByteArrayOutputStream`.

```

``````

ByteArrayOutputStream extracted = new ByteArrayOutputStream();
ArchiveLoadOptions options = new ArchiveLoadOptions();
options.setDecryptionPassword("p@s$");
try (Archive archive = new Archive("encrypted.zip", options)) {
try (InputStream decompressed = archive.getEntries().get(0).open()) {
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
extracted.write(b, 0, bytesRead);
} catch (IOException ex) {
}
}
 
```

This constructor does not decompress any entry. See [ArchiveEntry.open()](../../com.aspose.zip/archiveentry\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The fully qualified or the relative path to the archive file. |
| loadOptions | [ArchiveLoadOptions](../../com.aspose.zip/archiveloadoptions) | Options to load existing archive with. |

### Archive(String path, ArchiveLoadOptions loadOptions, ArchiveEntrySettings newEntrySettings) {#Archive-java.lang.String-com.aspose.zip.ArchiveLoadOptions-com.aspose.zip.ArchiveEntrySettings-}
```
public Archive(String path, ArchiveLoadOptions loadOptions, ArchiveEntrySettings newEntrySettings)
```


Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class and composes an entry list can be extracted from the archive.

The following example extracts an encrypted archive, then decompresses first entry to a `ByteArrayOutputStream`.

```

``````

     ByteArrayOutputStream extracted = new ByteArrayOutputStream();
     ArchiveLoadOptions options = new ArchiveLoadOptions();
     options.setDecryptionPassword("p@s$");
     try (Archive archive = new Archive("encrypted.zip", options)) {
         try (InputStream decompressed = archive.getEntries().get(0).open()) {
             byte[] b = new byte[8192];
             int bytesRead;
             while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
                 extracted.write(b, 0, bytesRead);
         } catch (IOException ex) {
         }
     }
 
```

Dieser Konstruktor dekomprimiert keinen Eintrag. Siehe die Methode [ArchiveEntry.open()](../../com.aspose.zip/archiveentry\\#open--) zum Dekomprimieren.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | java.lang.String | Der vollqualifizierte oder relative Pfad zur Archivdatei. |
| loadOptions | [ArchiveLoadOptions](../../com.aspose.zip/archiveloadoptions) | Optionen zum Laden eines bestehenden Archivs. |
| newEntrySettings | [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) | Kompressions- und Verschlüsselungseinstellungen, die für neu hinzugefügte [ArchiveEntry](../../com.aspose.zip/archiveentry)-Elemente verwendet werden. Wenn nicht angegeben, wird die am häufigsten verwendete Deflate-Kompression ohne Verschlüsselung verwendet. |

### Archive(String mainSegment, String[] segmentsInOrder) {#Archive-java.lang.String-java.lang.String---}
```
public Archive(String mainSegment, String[] segmentsInOrder)
```


Initialisiert eine neue Instanz der [Archive](../../com.aspose.zip/archive)-Klasse aus einem mehrteiligen ZIP-Archiv und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann.

```

``````

try (Archive a = new Archive("archive.zip", new String[] { "archive.z01", "archive.z02" })) {
a.extractToDirectory("destination");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| mainSegment | java.lang.String | Path to the last segment of multi-volume archive with the central directory.

Usually this segment has \*.zip extension and smaller than others. |
| segmentsInOrder | java.lang.String[] | Paths to each segment but the last of multi-volume zip archive respecting order.

Usually they named filename.z01, filename.z02, ..., filename.z(n-1). |

### Archive(String mainSegment, String[] segmentsInOrder, ArchiveLoadOptions loadOptions) {#Archive-java.lang.String-java.lang.String---com.aspose.zip.ArchiveLoadOptions-}
```
public Archive(String mainSegment, String[] segmentsInOrder, ArchiveLoadOptions loadOptions)
```


Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class from multi-volume ZIP archive and composes an entry list can be extracted from the archive.

This sample extract to a directory an archive of three segments.

```

``````

     try (Archive a = new Archive("archive.zip", new String[] { "archive.z01", "archive.z02" })) {
         a.extractToDirectory("destination");
     }
 
```



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | mainSegment | java.lang.String | Pfad zum letzten Segment eines mehrteiligen Archivs mit dem zentralen Verzeichnis. |

Normalerweise hat dieses Segment die Erweiterung \\*.zip und ist kleiner als die anderen. |
|  | segmentsInOrder | java.lang.String[] | Pfade zu jedem Segment außer dem letzten eines mehrteiligen Zip-Archivs in der richtigen Reihenfolge. |

Normalerweise werden sie filename.z01, filename.z02, ..., filename.z(n-1) genannt. |
| loadOptions | [ArchiveLoadOptions](../../com.aspose.zip/archiveloadoptions) | Optionen zum Laden eines bestehenden Archivs. |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final Archive createEntries(File directory)
```


Fügt dem Archiv alle Dateien und Verzeichnisse rekursiv aus dem angegebenen Verzeichnis hinzu.

```

``````

try (Archive archive = new Archive()) {
java.io.File folder = new java.io.File("C:\\folder");
archive.createEntries(folder);
archive.save("folder.zip");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | Directory to compress. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - The archive with entries composed.
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final Archive createEntries(File directory, boolean includeRootDirectory)
```


Add to the archive all files and directories recursively in the directory given.

```

``````

    try (Archive archive = new Archive()) {
        java.io.File folder = new java.io.File("C:\\folder");
        archive.createEntries(folder);
        archive.save("folder.zip");
    }
 
```



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Verzeichnis | java.io.File | Verzeichnis zum Komprimieren. |
| includeRootDirectory | boolean | Gibt an, ob das Stammverzeichnis selbst einbezogen werden soll oder nicht. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - The archive with entries composed.
### createEntries(String sourceDirectory) {#createEntries-java.lang.String-}
```
public final Archive createEntries(String sourceDirectory)
```


Fügt dem Archiv alle Dateien und Verzeichnisse rekursiv aus dem angegebenen Verzeichnis hinzu.

```

``````

try (Archive archive = new Archive()) {
archive.createEntries("C:\\folder");
archive.save("folder.zip");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | Directory to compress. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - The archive with entries composed.
### createEntries(String sourceDirectory, boolean includeRootDirectory) {#createEntries-java.lang.String-boolean-}
```
public final Archive createEntries(String sourceDirectory, boolean includeRootDirectory)
```


Add to the archive all files and directories recursively in the directory given.

```

``````

    try (Archive archive = new Archive()) {
        archive.createEntries("C:\\folder");
        archive.save("folder.zip");
    }
 
```



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Quellverzeichnis | java.lang.String | Verzeichnis zum Komprimieren. |
| includeRootDirectory | boolean | Gibt an, ob das Stammverzeichnis selbst einbezogen werden soll oder nicht. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - The archive with entries composed.
### createEntry(String name, File file) {#createEntry-java.lang.String-java.io.File-}
```
public final ArchiveEntry createEntry(String name, File file)
```


Erstellt einen einzelnen Eintrag im Archiv.

Erstellt ein Archiv mit Einträgen, die jeweils mit unterschiedlichen Verschlüsselungsmethoden und Passwörtern verschlüsselt sind.

```

``````

try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
java.io.File fi1 = new java.io.File("data1.bin");
java.io.File fi2 = new java.io.File("data2.bin");
java.io.File fi3 = new java.io.File("data3.bin");
try (Archive archive = new Archive()) {
archive.createEntry("entry1.bin", fi1, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")));
archive.createEntry("entry2.bin", fi2, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEncryptionSettings("pass2", EncryptionMethod.AES128)));
archive.createEntry("entry3.bin", fi3, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEncryptionSettings("pass3", EncryptionMethod.AES256)));
archive.save(zipFile);
}
} catch (IOException ignored) {
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `file` parameter does not affect the entry name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| file | java.io.File | The metadata of file to be compressed. |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, File file, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final ArchiveEntry createEntry(String name, File file, boolean openImmediately)
```


Creates a single entry within the archive.

Compose archive with entries encrypted with different encryption methods and passwords each.

```

``````

    try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
        java.io.File fi1 = new java.io.File("data1.bin");
        java.io.File fi2 = new java.io.File("data2.bin");
        java.io.File fi3 = new java.io.File("data3.bin");
        try (Archive archive = new Archive()) {
            archive.createEntry("entry1.bin", fi1, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")));
            archive.createEntry("entry2.bin", fi2, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEncryptionSettings("pass2", EncryptionMethod.AES128)));
            archive.createEntry("entry3.bin", fi3, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEncryptionSettings("pass3", EncryptionMethod.AES256)));
            archive.save(zipFile);
        }
    } catch (IOException ignored) {
    }
 
```

Der Eintragsname wird ausschließlich über den Parameter `name` festgelegt. Der im Parameter `file` angegebene Dateiname hat keinen Einfluss auf den Eintragsnamen.

Wenn die Datei sofort mit dem Parameter `openImmediately` geöffnet wird, ist sie gesperrt, bis das Archiv gespeichert wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String | Der Name des Eintrags. |
| Datei | java.io.File | Die Metadaten der zu komprimierenden Datei. |
| openImmediately | boolean | True, wenn die Datei sofort geöffnet wird, andernfalls wird die Datei beim Speichern des Archivs geöffnet. |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, File file, boolean openImmediately, ArchiveEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.io.File-boolean-com.aspose.zip.ArchiveEntrySettings-}
```
public final ArchiveEntry createEntry(String name, File file, boolean openImmediately, ArchiveEntrySettings newEntrySettings)
```


Erstellt einen einzelnen Eintrag im Archiv.

Erstellt ein Archiv mit Einträgen, die jeweils mit unterschiedlichen Verschlüsselungsmethoden und Passwörtern verschlüsselt sind.

```

``````

try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
java.io.File fi1 = new java.io.File("data1.bin");
java.io.File fi2 = new java.io.File("data2.bin");
java.io.File fi3 = new java.io.File("data3.bin");
try (Archive archive = new Archive()) {
archive.createEntry("entry1.bin", fi1, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")));
archive.createEntry("entry2.bin", fi2, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEncryptionSettings("pass2", EncryptionMethod.AES128)));
archive.createEntry("entry3.bin", fi3, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEncryptionSettings("pass3", EncryptionMethod.AES256)));
archive.save(zipFile);
}
} catch (IOException ignored) {
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `file` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is saved.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| file | java.io.File | The metadata of file to be compressed. |
| openImmediately | boolean | True, if open the file immediately, otherwise open the file on archive saving. |
| newEntrySettings | [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) | Compression and encryption settings used for added [ArchiveEntry](../../com.aspose.zip/archiveentry) item. |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final ArchiveEntry createEntry(String name, InputStream source)
```


Creates a single entry within the archive.

```

``````

     try (Archive archive = new Archive(new ArchiveEntrySettings(null, new AesEncryptionSettings("p@s$", EncryptionMethod.AES256)))) {
         archive.createEntry("data.bin", new ByteArrayInputStream(new byte[] {
                 0x00,
                 (byte) 0xFF
         }));
         archive.save("archive.zip");
     }
 
```



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String | Der Name des Eintrags. |
| source | java.io.InputStream | Der Eingabestream für den Eintrag. |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, InputStream source, ArchiveEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.ArchiveEntrySettings-}
```
public final ArchiveEntry createEntry(String name, InputStream source, ArchiveEntrySettings newEntrySettings)
```


Erstellt einen einzelnen Eintrag im Archiv.

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(null, new AesEncryptionSettings(\"p@s$\", EncryptionMethod.AES256)))) {
archive.createEntry(\"data.bin\", new ByteArrayInputStream(new byte[] {
0x00,
(byte) 0xFF
}));
archive.save("archive.zip");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| source | java.io.InputStream | The input stream for the entry. |
| newEntrySettings | [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) | Compression and encryption settings used for added [ArchiveEntry](../../com.aspose.zip/archiveentry) item. |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, InputStream source, ArchiveEntrySettings newEntrySettings, File file) {#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.ArchiveEntrySettings-java.io.File-}
```
public final ArchiveEntry createEntry(String name, InputStream source, ArchiveEntrySettings newEntrySettings, File file)
```


Creates a single entry within the archive.

Compose archive with encrypted entry.

```

``````

    try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
        try (Archive archive = new Archive()) {
            archive.createEntry("entry1.bin", new ByteArrayInputStream(new byte[] {
                    0x00,
                    (byte) 0xFF
            }), new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")), new java.io.File("data1.bin"));
            archive.save(zipFile);
        }
    } catch (IOException ignored) {
    }
 
```

Der Eintragsname wird ausschließlich über den Parameter `name` festgelegt. Der im Parameter `file` angegebene Dateiname hat keinen Einfluss auf den Eintragsnamen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String | Der Name des Eintrags. |
| source | java.io.InputStream | Der Eingabestream für den Eintrag. |
| newEntrySettings | [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) | Komprimierungs- und Verschlüsselungseinstellungen, die für das hinzugefügte [ArchiveEntry](../../com.aspose.zip/archiveentry)-Element verwendet werden. |
| Datei | java.io.File | Die Metadaten der zu komprimierenden Datei oder des Ordners. |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, String path) {#createEntry-java.lang.String-java.lang.String-}
```
public final ArchiveEntry createEntry(String name, String path)
```


Erstellt einen einzelnen Eintrag im Archiv.

```

``````

try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
try (Archive archive = new Archive()) {
archive.createEntry("data.bin", "file.dat");
archive.save(zipFile);
}
} catch (IOException ex) {
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `path` parameter does not affect the entry name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| path | java.lang.String | The fully qualified name of the new file, or the relative file name to be compressed. |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, String path, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final ArchiveEntry createEntry(String name, String path, boolean openImmediately)
```


Creates a single entry within the archive.

```

``````

     try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
         try (Archive archive = new Archive()) {
             archive.createEntry("data.bin", "file.dat");
             archive.save(zipFile);
         }
     } catch (IOException ex) {
     }
 
```

Der Eintragsname wird ausschließlich im Parameter `name` festgelegt. Der im Parameter `path` angegebene Dateiname beeinflusst den Eintragsnamen nicht.

Wenn die Datei sofort mit dem Parameter `openImmediately` geöffnet wird, ist sie gesperrt, bis das Archiv gespeichert wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String | Der Name des Eintrags. |
| path | java.lang.String | Der vollqualifizierte Name der neuen Datei oder der relative Dateiname, der komprimiert werden soll. |
| openImmediately | boolean | True, wenn die Datei sofort geöffnet wird, andernfalls wird die Datei beim Speichern des Archivs geöffnet. |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, String path, boolean openImmediately, ArchiveEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.lang.String-boolean-com.aspose.zip.ArchiveEntrySettings-}
```
public final ArchiveEntry createEntry(String name, String path, boolean openImmediately, ArchiveEntrySettings newEntrySettings)
```


Erstellt einen einzelnen Eintrag im Archiv.

```

``````

try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
try (Archive archive = new Archive()) {
archive.createEntry("data.bin", "file.dat");
archive.save(zipFile);
}
} catch (IOException ex) {
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `path` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is saved.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| path | java.lang.String | The fully qualified name of the new file, or the relative file name to be compressed. |
| openImmediately | boolean | True, if open the file immediately, otherwise open the file on archive saving. |
| newEntrySettings | [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) | Compression and encryption settings used for added [ArchiveEntry](../../com.aspose.zip/archiveentry) item. |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, Supplier&lt;InputStream&gt; streamProvider) {#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--}
```
public final ArchiveEntry createEntry(String name, Supplier<InputStream> streamProvider)
```


Creates a single entry within the archive.

Compose archive with encrypted entry.

```

``````

     Supplier<InputStream> provider = new Supplier<InputStream>() {
         public InputStream get() {
             return new ByteArrayInputStream(new byte[] {(byte) 0xFF, 0x00});
         }
     };
     try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
         try (Archive archive = new Archive()) {
             archive.createEntry("entry1.bin", provider, new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")));
             archive.save(zipFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String | der Name des Eintrags |
| streamProvider | java.util.function.Supplier&lt;java.io.InputStream&gt; | die Methode, die den Eingabestream für den Eintrag bereitstellt |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - zip entry instance
### createEntry(String name, Supplier&lt;InputStream&gt; streamProvider, ArchiveEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--com.aspose.zip.ArchiveEntrySettings-}
```
public final ArchiveEntry createEntry(String name, Supplier<InputStream> streamProvider, ArchiveEntrySettings newEntrySettings)
```


Erstellt einen einzelnen Eintrag im Archiv.

Archiv mit verschlüsseltem Eintrag erstellen.

```

``````

Supplier<InputStream> provider = new Supplier<InputStream>() {
public InputStream get() {
return new ByteArrayInputStream(new byte[] {(byte) 0xFF, 0x00});
}
};
try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
try (Archive archive = new Archive()) {
archive.createEntry(\"entry1.bin\", provider, new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings(\"pass1\")));
archive.save(zipFile);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| streamProvider | java.util.function.Supplier&lt;java.io.InputStream&gt; | the method providing input stream for the entry |
| newEntrySettings | [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) | compression and encryption settings used for added [ArchiveEntry](../../com.aspose.zip/archiveentry) item |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - zip entry instance
### deleteEntry(ArchiveEntry entry) {#deleteEntry-com.aspose.zip.ArchiveEntry-}
```
public final Archive deleteEntry(ArchiveEntry entry)
```


Removes the first occurrence of the specific entry from the entry list.

Here is how you can remove all entries except the last one:

```

``````

    try (Archive archive = new Archive("archive.zip")) {
        while (archive.getEntries().size() > 1)
            archive.deleteEntry(archive.getEntries().get(0));
        archive.save("last_entry.zip");
    }
 
```



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| entry | [ArchiveEntry](../../com.aspose.zip/archiveentry) | Der Eintrag, der aus der Eintragsliste entfernt werden soll. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - The archive with the entry deleted.
### deleteEntry(int entryIndex) {#deleteEntry-int-}
```
public final Archive deleteEntry(int entryIndex)
```


Entfernt den Eintrag aus der Eintragsliste anhand des Index.

```

``````

try (Archive archive = new Archive("two_files.zip")) {
archive.deleteEntry(0);
archive.save("single_file.zip");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| entryIndex | int | The zero-based index of the entry to remove. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - The archive with the entry deleted.
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all the files in the archive to the directory provided.

```

``````

    try (Archive archive = new Archive("archive.zip")) {
        archive.extractToDirectory("C:\\extracted");
    }
 
```

Wenn das Verzeichnis nicht existiert, wird es erstellt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| destinationDirectory | java.lang.String | Der Pfad zum Verzeichnis, in dem die extrahierten Dateien abgelegt werden sollen. |

### getComment() {#getComment--}
```
public final String getComment()
```


Liefert den Kommentar für das gesamte Archiv.

Wenn `ArchiveLoadOptions.Encoding`([ArchiveLoadOptions.getEncoding](../../com.aspose.zip/archiveloadoptions\#getEncoding)/[ArchiveLoadOptions.setEncoding](../../com.aspose.zip/archiveloadoptions\#setEncoding)) angegeben ist, wird damit dekodiert. Andernfalls wird UTF-8 verwendet.

**Returns:**
java.lang.String - Kommentar für das gesamte Archiv.
### getEntries() {#getEntries--}
```
public final List<ArchiveEntry> getEntries()
```


Liefert Einträge vom Typ [ArchiveEntry](../../com.aspose.zip/archiveentry), die das Archiv bilden.

**Returns:**
java.util.List&lt;com.aspose.zip.ArchiveEntry&gt; - Einträge vom Typ [ArchiveEntry](../../com.aspose.zip/archiveentry), die das Archiv bilden.
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Ruft Einträge vom Typ [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) ab, die das Archiv bilden.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - Einträge vom Typ [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), die das Archiv bilden.
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Liefert das Archivformat (Zip)

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - Zip archive format.
### getNewEntrySettings() {#getNewEntrySettings--}
```
public final ArchiveEntrySettings getNewEntrySettings()
```


Kompressions- und Verschlüsselungseinstellungen, die für neu hinzugefügte [ArchiveEntry](../../com.aspose.zip/archiveentry)-Elemente verwendet werden.

**Returns:**
[ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) - the [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) instance
### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


Speichert das Archiv in den angegebenen Stream.

```

``````

try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
try (Archive archive = new Archive()) {
archive.createEntry("entry.bin", "data.bin");
archive.save(zipFile);
}
} catch (IOException ex) {
}
 
```

`outputStream` must be writable.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outputStream | java.io.OutputStream | Destination stream. |

### save(OutputStream outputStream, ArchiveSaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.ArchiveSaveOptions-}
```
public final void save(OutputStream outputStream, ArchiveSaveOptions saveOptions)
```


Saves archive to the stream provided.

```

``````

    try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
        try (Archive archive = new Archive()) {
            archive.createEntry("entry.bin", "data.bin");
            archive.save(zipFile);
        }
    } catch (IOException ex) {
    }
 
```

`outputStream` muss beschreibbar sein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| outputStream | java.io.OutputStream | Ziel-Stream. |
| saveOptions | [ArchiveSaveOptions](../../com.aspose.zip/archivesaveoptions) | Optionen zum Speichern des Archivs. |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Speichert das Archiv in die angegebene Zieldatei.

```

``````

try (Archive archive = new Archive()) {
archive.createEntry("entry.bin", "data.bin");
ArchiveSaveOptions options = new ArchiveSaveOptions();
options.setEncoding(StandardCharsets.US_ASCII);
archive.save("archive.zip", options);
}
 
```

It is possible to save an archive to the same path as it was loaded from. However, this is not recommended because this approach uses copying to temporary file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |

### save(String destinationFileName, ArchiveSaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.ArchiveSaveOptions-}
```
public final void save(String destinationFileName, ArchiveSaveOptions saveOptions)
```


Saves archive to the destination file provided.

```

``````

    try (Archive archive = new Archive()) {
        archive.createEntry("entry.bin", "data.bin");
        ArchiveSaveOptions options = new ArchiveSaveOptions();
        options.setEncoding(StandardCharsets.US_ASCII);
        archive.save("archive.zip", options);
    }
 
```

Es ist möglich, ein Archiv am selben Pfad zu speichern, von dem es geladen wurde. Dies wird jedoch nicht empfohlen, da dieser Ansatz das Kopieren in eine temporäre Datei verwendet.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| destinationFileName | java.lang.String | Der Pfad des zu erstellenden Archivs. Wenn der angegebene Dateiname auf eine bereits vorhandene Datei zeigt, wird diese überschrieben. |
| saveOptions | [ArchiveSaveOptions](../../com.aspose.zip/archivesaveoptions) | Optionen zum Speichern des Archivs. |

### saveSplit(String destinationDirectory, SplitArchiveSaveOptions options) {#saveSplit-java.lang.String-com.aspose.zip.SplitArchiveSaveOptions-}
```
public final void saveSplit(String destinationDirectory, SplitArchiveSaveOptions options)
```


Speichert ein mehrteiliges Archiv in das angegebene Zielverzeichnis.

```

``````

try (Archive archive = new Archive()) {
archive.createEntry("entry.bin", "data.bin");
archive.saveSplit( "C:\\Folder", new SplitArchiveSaveOptions("volume", 65536));
}
 
```

This method composes several (n) files filename.z01, filename.z02, ..., filename.z(n-1), filename.zip.

Cannot make existing archive multi-volume.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | The path to the directory where archive segments to be created. |
| options | [SplitArchiveSaveOptions](../../com.aspose.zip/splitarchivesaveoptions) | Options for archive saving, including file name. |

