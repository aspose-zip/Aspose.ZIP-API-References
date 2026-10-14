---
title: "SharArchive"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Diese Klasse repräsentiert eine Shar-Archivdatei."
type: docs
weight: 119
url: /de/java/com.aspose.zip/shararchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.AutoCloseable
```
public class SharArchive implements AutoCloseable
```

Diese Klasse repräsentiert eine Shar-Archivdatei.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [SharArchive()](#SharArchive--) | Initialisiert eine neue Instanz der Klasse [SharArchive](../../com.aspose.zip/shararchive). |
| [SharArchive(String path)](#SharArchive-java.lang.String-) | Initialisiert eine neue Instanz der Klasse [SharArchive](../../com.aspose.zip/shararchive), die zum Dekomprimieren vorbereitet ist. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | Fügt dem Archiv alle Dateien und Verzeichnisse rekursiv im angegebenen Verzeichnis hinzu. |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | Fügt dem Archiv alle Dateien und Verzeichnisse rekursiv im angegebenen Verzeichnis hinzu. |
| [createEntries(String sourceDirectory)](#createEntries-java.lang.String-) | Fügt dem Archiv alle Dateien und Verzeichnisse rekursiv im angegebenen Verzeichnis hinzu. |
| [createEntries(String sourceDirectory, boolean includeRootDirectory)](#createEntries-java.lang.String-boolean-) | Fügt dem Archiv alle Dateien und Verzeichnisse rekursiv im angegebenen Verzeichnis hinzu. |
| [createEntry(String name, File file)](#createEntry-java.lang.String-java.io.File-) | Erstellt einen einzelnen Eintrag im Archiv. |
| [createEntry(String name, File file, boolean includeRootDirectory)](#createEntry-java.lang.String-java.io.File-boolean-) | Erstellen Sie einen einzelnen Eintrag im Archiv. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | Erstellen Sie einen einzelnen Eintrag im Archiv. |
| [createEntry(String name, String sourcePath)](#createEntry-java.lang.String-java.lang.String-) | Erstellen Sie einen einzelnen Eintrag im Archiv. |
| [createEntry(String name, String sourcePath, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | Erstellen Sie einen einzelnen Eintrag im Archiv. |
| [deleteEntry(SharEntry entry)](#deleteEntry-com.aspose.zip.SharEntry-) | Entfernt das erste Vorkommen eines bestimmten Eintrags aus der Eintragsliste. |
| [deleteEntry(int entryIndex)](#deleteEntry-int-) | Entfernt den Eintrag aus der Eintragsliste anhand des Index. |
| [getEntries()](#getEntries--) | Liefert Einträge vom Typ [SharEntry](../../com.aspose.zip/sharentry), die das Archiv bilden. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Speichert das Archiv in den angegebenen Stream. |
| [save(String destinationFileName)](#save-java.lang.String-) | Speichert das Archiv in die angegebene Zieldatei. |
### SharArchive() {#SharArchive--}
```
public SharArchive()
```


Initialisiert eine neue Instanz der Klasse [SharArchive](../../com.aspose.zip/shararchive).

Das folgende Beispiel zeigt, wie man eine Datei komprimiert.

```

``````

try (SharArchive archive = new SharArchive()) {
archive.createEntry("first.bin", "data.bin");
archive.save("archive.shar");
}
 
```



### SharArchive(String path) {#SharArchive-java.lang.String-}
```
public SharArchive(String path)
```


Initializes a new instance of the [SharArchive](../../com.aspose.zip/shararchive) class prepared for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the source of the archive |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final SharArchive createEntries(File directory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream sharFile = new FileOutputStream("archive.shar")) {
         try (SharArchive archive = new SharArchive()) {
             archive.createEntries(new java.io.File("C:\\folder"), false);
             archive.save(sharFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Verzeichnis | java.io.File | das Verzeichnis zum Komprimieren |

**Returns:**
[SharArchive](../../com.aspose.zip/shararchive) - Shar entry instance
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final SharArchive createEntries(File directory, boolean includeRootDirectory)
```


Fügt dem Archiv alle Dateien und Verzeichnisse rekursiv im angegebenen Verzeichnis hinzu.

```

``````

try (FileOutputStream sharFile = new FileOutputStream("archive.shar")) {
try (SharArchive archive = new SharArchive()) {
archive.createEntries(new java.io.File("C:\\folder"), false);
archive.save(sharFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | the directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[SharArchive](../../com.aspose.zip/shararchive) - Shar entry instance
### createEntries(String sourceDirectory) {#createEntries-java.lang.String-}
```
public final SharArchive createEntries(String sourceDirectory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream sharFile = new FileOutputStream("archive.shar")) {
         try (SharArchive archive = new SharArchive()) {
             archive.createEntries("C:\\folder", false);
             archive.save(sharFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Quellverzeichnis | java.lang.String | das Verzeichnis zum Komprimieren |

**Returns:**
[SharArchive](../../com.aspose.zip/shararchive) - Shar entry instance
### createEntries(String sourceDirectory, boolean includeRootDirectory) {#createEntries-java.lang.String-boolean-}
```
public final SharArchive createEntries(String sourceDirectory, boolean includeRootDirectory)
```


Fügt dem Archiv alle Dateien und Verzeichnisse rekursiv im angegebenen Verzeichnis hinzu.

```

``````

try (FileOutputStream sharFile = new FileOutputStream("archive.shar")) {
try (SharArchive archive = new SharArchive()) {
archive.createEntries("C:\\folder", false);
archive.save(sharFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | the directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[SharArchive](../../com.aspose.zip/shararchive) - Shar entry instance
### createEntry(String name, File file) {#createEntry-java.lang.String-java.io.File-}
```
public final SharEntry createEntry(String name, File file)
```


Creates a single entry within the archive.

```

``````

     java.io.File file = new java.io.File("data.bin");
     try (SharArchive archive = new SharArchive()) {
         archive.createEntry("test.bin", file);
         archive.save("archive.shar");
     }
 
```



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String | der Name des Eintrags |
| Datei | java.io.File | die Metadaten der Datei oder des Ordners, die komprimiert werden sollen |

**Returns:**
[SharEntry](../../com.aspose.zip/sharentry) - Shar entry instance
### createEntry(String name, File file, boolean includeRootDirectory) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final SharEntry createEntry(String name, File file, boolean includeRootDirectory)
```


Erstellen Sie einen einzelnen Eintrag im Archiv.

```

``````

java.io.File file = new java.io.File("data.bin");
try (SharArchive archive = new SharArchive()) {
archive.createEntry("test.bin", file);
archive.save("archive.shar");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file or folder to be compressed |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[SharEntry](../../com.aspose.zip/sharentry) - Shar entry instance
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final SharEntry createEntry(String name, InputStream source)
```


Create a single entry within the archive.

```

``````

     try (SharArchive archive = new SharArchive()) {
         archive.createEntry("data.bin", new FileInputStream("data.bin"));
         archive.save("archive.shar");
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String | der Name des Eintrags |
| source | java.io.InputStream | der Eingabestream für den Eintrag |

**Returns:**
[SharEntry](../../com.aspose.zip/sharentry) - Shar entry instance
### createEntry(String name, String sourcePath) {#createEntry-java.lang.String-java.lang.String-}
```
public final SharEntry createEntry(String name, String sourcePath)
```


Erstellen Sie einen einzelnen Eintrag im Archiv.

```

``````

try (SharArchive archive = new SharArchive()) {
archive.createEntry("first.bin", "data.bin");
archive.save("archive.shar");
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `sourcePath` parameter does not affect the entry name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| sourcePath | java.lang.String | the path to the file to be compressed |

**Returns:**
[SharEntry](../../com.aspose.zip/sharentry) - Shar entry instance
### createEntry(String name, String sourcePath, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final SharEntry createEntry(String name, String sourcePath, boolean openImmediately)
```


Create a single entry within the archive.

```

``````

     try (SharArchive archive = new SharArchive()) {
         archive.createEntry("first.bin", "data.bin");
         archive.save("archive.shar");
     }
 
```

Der Eintragsname wird ausschließlich im Parameter `name` festgelegt. Der im Parameter `sourcePath` angegebene Dateiname hat keinen Einfluss auf den Eintragsnamen.

Wenn die Datei sofort mit dem Parameter `openImmediately` geöffnet wird, bleibt sie gesperrt, bis das Archiv freigegeben wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String | der Name des Eintrags |
| sourcePath | java.lang.String | der Pfad zur zu komprimierenden Datei |
| openImmediately | boolean | true, wenn die Datei sofort geöffnet werden soll, andernfalls wird die Datei beim Speichern des Archivs geöffnet |

**Returns:**
[SharEntry](../../com.aspose.zip/sharentry) - Shar entry instance
### deleteEntry(SharEntry entry) {#deleteEntry-com.aspose.zip.SharEntry-}
```
public final SharArchive deleteEntry(SharEntry entry)
```


Entfernt das erste Vorkommen eines bestimmten Eintrags aus der Eintragsliste.

So können Sie alle Einträge außer dem letzten entfernen:

```

``````

try (SharArchive archive = new SharArchive("archive.shar")) {
while (archive.getEntries().size() > 1)
archive.deleteEntry(archive.getEntries().get(0));
archive.save("outputSharFile.shar");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| entry | [SharEntry](../../com.aspose.zip/sharentry) | the entry to remove from the entries list |

**Returns:**
[SharArchive](../../com.aspose.zip/shararchive) - Shar entry instance
### deleteEntry(int entryIndex) {#deleteEntry-int-}
```
public final SharArchive deleteEntry(int entryIndex)
```


Removes the entry from the entry list by index.

```

``````

     try (SharArchive archive = new SharArchive("two_files.shar")) {
         archive.deleteEntry(0);
         archive.save("single_file.shar");
     }
 
```



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| entryIndex | int | der nullbasierte Index des zu entfernenden Eintrags |

**Returns:**
[SharArchive](../../com.aspose.zip/shararchive) - the archive with the entry deleted
### getEntries() {#getEntries--}
```
public final List<SharEntry> getEntries()
```


Liefert Einträge vom Typ [SharEntry](../../com.aspose.zip/sharentry), die das Archiv bilden.

**Returns:**
java.util.List&lt;com.aspose.zip.SharEntry&gt; - Einträge vom Typ [SharEntry](../../com.aspose.zip/sharentry), die das Archiv bilden
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Speichert das Archiv in den angegebenen Stream.

```

``````

try (FileOutputStream sharFile = new FileOutputStream("archive.shar")) {
try (SharArchive archive = new SharArchive()) {
archive.createEntry("entry1", "data.bin");
archive.save(sharFile);
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


Saves archive to the destination file provided.

```

``````

     try (SharArchive archive = new SharArchive()) {
         archive.createEntry("entry1", "data.bin");
         archive.save("archive.shar");
     }
 
```



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | destinationFileName | java.lang.String | Der Pfad des zu erstellenden Archivs. Wenn der angegebene Dateiname auf eine bereits vorhandene Datei verweist, wird diese überschrieben. |

Es ist möglich, ein Archiv am selben Pfad zu speichern, von dem es geladen wurde. Dies wird jedoch nicht empfohlen, da dieser Ansatz das Kopieren in eine temporäre Datei erfordert |

