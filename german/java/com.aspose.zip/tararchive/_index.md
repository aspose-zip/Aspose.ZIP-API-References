---
title: "TarArchive"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Diese Klasse repräsentiert eine Tar-Archivdatei."
type: docs
weight: 125
url: /de/java/com.aspose.zip/tararchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class TarArchive implements IArchive, AutoCloseable
```

Diese Klasse repräsentiert eine Tar-Archivdatei. Verwenden Sie sie, um Tar-Archive zu erstellen, zu extrahieren oder zu aktualisieren.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [TarArchive()](#TarArchive--) | Initialisiert eine neue Instanz der Klasse [TarArchive](../../com.aspose.zip/tararchive). |
| [TarArchive(InputStream sourceStream)](#TarArchive-java.io.InputStream-) | Initialisiert eine neue Instanz der [Archive](../../com.aspose.zip/archive)-Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann. |
| [TarArchive(String path)](#TarArchive-java.lang.String-) | Initialisiert eine neue Instanz der Klasse [TarArchive](../../com.aspose.zip/tararchive) und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | Fügt dem Archiv alle Dateien und Verzeichnisse rekursiv im angegebenen Verzeichnis hinzu. |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | Fügt dem Archiv alle Dateien und Verzeichnisse rekursiv im angegebenen Verzeichnis hinzu. |
| [createEntries(String sourceDirectory)](#createEntries-java.lang.String-) | Fügt dem Archiv alle Dateien und Verzeichnisse rekursiv im angegebenen Verzeichnis hinzu. |
| [createEntries(String sourceDirectory, boolean includeRootDirectory)](#createEntries-java.lang.String-boolean-) | Fügt dem Archiv alle Dateien und Verzeichnisse rekursiv im angegebenen Verzeichnis hinzu. |
| [createEntry(String name, File file)](#createEntry-java.lang.String-java.io.File-) | Erstellt einen einzelnen Eintrag im Archiv. |
| [createEntry(String name, File file, boolean openImmediately)](#createEntry-java.lang.String-java.io.File-boolean-) | Erstellt einen einzelnen Eintrag im Archiv. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | Erstellt einen einzelnen Eintrag im Archiv. |
| [createEntry(String name, InputStream source, File file)](#createEntry-java.lang.String-java.io.InputStream-java.io.File-) | Erstellt einen einzelnen Eintrag im Archiv. |
| [createEntry(String name, String path)](#createEntry-java.lang.String-java.lang.String-) | Erstellt einen einzelnen Eintrag im Archiv. |
| [createEntry(String name, String path, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | Erstellt einen einzelnen Eintrag im Archiv. |
| [deleteEntry(TarEntry entry)](#deleteEntry-com.aspose.zip.TarEntry-) | Entfernt das erste Vorkommen eines bestimmten Eintrags aus der Eintragsliste. |
| [deleteEntry(int entryIndex)](#deleteEntry-int-) | Entfernt den Eintrag aus der Eintragsliste anhand des Index. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrahiert alle Dateien im Archiv in das angegebene Verzeichnis. |
| [fromGZip(InputStream source)](#fromGZip-java.io.InputStream-) | Extrahiert das bereitgestellte gzip-Archiv und erstellt ein [TarArchive](../../com.aspose.zip/tararchive) aus den extrahierten Daten. |
| [fromGZip(String path)](#fromGZip-java.lang.String-) | Extrahiert das bereitgestellte gzip-Archiv und erstellt ein [TarArchive](../../com.aspose.zip/tararchive) aus den extrahierten Daten. |
| [fromLZ4(InputStream source)](#fromLZ4-java.io.InputStream-) | Extrahiert das bereitgestellte LZ4-Archiv und erstellt ein [TarArchive](../../com.aspose.zip/tararchive) aus den extrahierten Daten. |
| [fromLZ4(String path)](#fromLZ4-java.lang.String-) | Extrahiert das bereitgestellte LZ4-Archiv und erstellt ein [TarArchive](../../com.aspose.zip/tararchive) aus den extrahierten Daten. |
| [fromLZMA(InputStream source)](#fromLZMA-java.io.InputStream-) | Extrahiert das bereitgestellte LZMA-Archiv und erstellt ein [TarArchive](../../com.aspose.zip/tararchive) aus den extrahierten Daten. |
| [fromLZMA(String path)](#fromLZMA-java.lang.String-) | Extrahiert das bereitgestellte LZMA-Archiv und erstellt ein [TarArchive](../../com.aspose.zip/tararchive) aus den extrahierten Daten. |
| [fromLZip(InputStream source)](#fromLZip-java.io.InputStream-) | Extrahiert das bereitgestellte lzip-Archiv und erstellt ein [TarArchive](../../com.aspose.zip/tararchive) aus den extrahierten Daten. |
| [fromLZip(String path)](#fromLZip-java.lang.String-) | Extrahiert das bereitgestellte lzip-Archiv und erstellt ein [TarArchive](../../com.aspose.zip/tararchive) aus den extrahierten Daten. |
| [fromXz(InputStream source)](#fromXz-java.io.InputStream-) | Extrahiert das bereitgestellte xz-Format-Archiv und erstellt ein [TarArchive](../../com.aspose.zip/tararchive) aus den extrahierten Daten. |
| [fromXz(String path)](#fromXz-java.lang.String-) | Extrahiert das bereitgestellte xz-Format-Archiv und erstellt ein [TarArchive](../../com.aspose.zip/tararchive) aus den extrahierten Daten. |
| [fromZ(InputStream source)](#fromZ-java.io.InputStream-) | Extrahiert das bereitgestellte Z-Format-Archiv und erstellt ein [TarArchive](../../com.aspose.zip/tararchive) aus den extrahierten Daten. |
| [fromZ(String path)](#fromZ-java.lang.String-) | Extrahiert das bereitgestellte Z-Format-Archiv und erstellt ein [TarArchive](../../com.aspose.zip/tararchive) aus den extrahierten Daten. |
| [fromZstandard(InputStream source)](#fromZstandard-java.io.InputStream-) | Extrahiert das bereitgestellte Zstandard-Archiv und erstellt ein [TarArchive](../../com.aspose.zip/tararchive) aus den extrahierten Daten. |
| [fromZstandard(String path)](#fromZstandard-java.lang.String-) | Extrahiert das bereitgestellte Zstandard-Archiv und erstellt ein [TarArchive](../../com.aspose.zip/tararchive) aus den extrahierten Daten. |
| [getEntries()](#getEntries--) | Ruft Einträge des Typs [TarEntry](../../com.aspose.zip/tarentry) ab, die das Archiv bilden. |
| [getFileEntries()](#getFileEntries--) | Ruft Einträge des Typs [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) ab, die das Tar-Archiv bilden. |
| [getFormat()](#getFormat--) | Liefert das Archivformat. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Speichert das Archiv in den angegebenen Stream. |
| [save(OutputStream output, TarFormat format)](#save-java.io.OutputStream-com.aspose.zip.TarFormat-) | Speichert das Archiv in den angegebenen Stream. |
| [save(String destinationFileName)](#save-java.lang.String-) | Speichert das Archiv in die angegebene Zieldatei. |
| [save(String destinationFileName, TarFormat format)](#save-java.lang.String-com.aspose.zip.TarFormat-) | Speichert das Archiv in die angegebene Zieldatei. |
| [saveGzipped(OutputStream output)](#saveGzipped-java.io.OutputStream-) | Speichert das Archiv in den Stream mit gzip-Kompression. |
| [saveGzipped(OutputStream output, TarFormat format)](#saveGzipped-java.io.OutputStream-com.aspose.zip.TarFormat-) | Speichert das Archiv in den Stream mit gzip-Kompression. |
| [saveGzipped(String path)](#saveGzipped-java.lang.String-) | Speichert das Archiv in die Datei über den Pfad mit gzip-Kompression. |
| [saveGzipped(String path, TarFormat format)](#saveGzipped-java.lang.String-com.aspose.zip.TarFormat-) | Speichert das Archiv in die Datei über den Pfad mit gzip-Kompression. |
| [saveLZ4Compressed(OutputStream output)](#saveLZ4Compressed-java.io.OutputStream-) | Speichert das Archiv im Stream mit LZ4-Kompression. |
| [saveLZ4Compressed(OutputStream output, TarFormat format)](#saveLZ4Compressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | Speichert das Archiv im Stream mit LZ4-Kompression. |
| [saveLZ4Compressed(String path)](#saveLZ4Compressed-java.lang.String-) | Speichert das Archiv in die Datei über den Pfad mit LZ4-Kompression. |
| [saveLZ4Compressed(String path, TarFormat format)](#saveLZ4Compressed-java.lang.String-com.aspose.zip.TarFormat-) | Speichert das Archiv in die Datei über den Pfad mit LZ4-Kompression. |
| [saveLZMACompressed(OutputStream output)](#saveLZMACompressed-java.io.OutputStream-) | Speichert das Archiv im Stream mit LZMA-Kompression. |
| [saveLZMACompressed(OutputStream output, TarFormat format)](#saveLZMACompressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | Speichert das Archiv im Stream mit LZMA-Kompression. |
| [saveLZMACompressed(String path)](#saveLZMACompressed-java.lang.String-) | Speichert das Archiv in die Datei über den Pfad mit lzma-Kompression. |
| [saveLZMACompressed(String path, TarFormat format)](#saveLZMACompressed-java.lang.String-com.aspose.zip.TarFormat-) | Speichert das Archiv in die Datei über den Pfad mit lzma-Kompression. |
| [saveLzipped(OutputStream output)](#saveLzipped-java.io.OutputStream-) | Speichert das Archiv in den Stream mit lzip-Kompression. |
| [saveLzipped(OutputStream output, TarFormat format)](#saveLzipped-java.io.OutputStream-com.aspose.zip.TarFormat-) | Speichert das Archiv in den Stream mit lzip-Kompression. |
| [saveLzipped(String path)](#saveLzipped-java.lang.String-) | Speichert das Archiv in die Datei über den Pfad mit lzip-Kompression. |
| [saveLzipped(String path, TarFormat format)](#saveLzipped-java.lang.String-com.aspose.zip.TarFormat-) | Speichert das Archiv in die Datei über den Pfad mit lzip-Kompression. |
| [saveXzCompressed(OutputStream output)](#saveXzCompressed-java.io.OutputStream-) | Speichert das Archiv in den Stream mit xz-Kompression. |
| [saveXzCompressed(OutputStream output, TarFormat format)](#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | Speichert das Archiv in den Stream mit xz-Kompression. |
| [saveXzCompressed(OutputStream output, TarFormat format, XzArchiveSettings settings)](#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-) | Speichert das Archiv in den Stream mit xz-Kompression. |
| [saveXzCompressed(String path)](#saveXzCompressed-java.lang.String-) | Speichert das Archiv in die Datei über den Pfad mit xz-Kompression. |
| [saveXzCompressed(String path, TarFormat format)](#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-) | Speichert das Archiv in die Datei über den Pfad mit xz-Kompression. |
| [saveXzCompressed(String path, TarFormat format, XzArchiveSettings settings)](#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-) | Speichert das Archiv in die Datei über den Pfad mit xz-Kompression. |
| [saveZCompressed(OutputStream output)](#saveZCompressed-java.io.OutputStream-) | Speichert das Archiv in den Stream mit Z-Kompression. |
| [saveZCompressed(OutputStream output, TarFormat format)](#saveZCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | Speichert das Archiv in den Stream mit Z-Kompression. |
| [saveZCompressed(String path)](#saveZCompressed-java.lang.String-) | Speichert das Archiv in die Datei über den Pfad mit Z-Kompression. |
| [saveZCompressed(String path, TarFormat format)](#saveZCompressed-java.lang.String-com.aspose.zip.TarFormat-) | Speichert das Archiv in die Datei über den Pfad mit Z-Kompression. |
| [saveZstandard(OutputStream output)](#saveZstandard-java.io.OutputStream-) | Speichert das Archiv in den Stream mit Zstandard-Kompression. |
| [saveZstandard(OutputStream output, TarFormat format)](#saveZstandard-java.io.OutputStream-com.aspose.zip.TarFormat-) | Speichert das Archiv in den Stream mit Zstandard-Kompression. |
| [saveZstandard(String path)](#saveZstandard-java.lang.String-) | Speichert das Archiv in die Datei über den Pfad mit Zstandard-Kompression. |
| [saveZstandard(String path, TarFormat format)](#saveZstandard-java.lang.String-com.aspose.zip.TarFormat-) | Speichert das Archiv in die Datei über den Pfad mit Zstandard-Kompression. |
### TarArchive() {#TarArchive--}
```
public TarArchive()
```


Initialisiert eine neue Instanz der Klasse [TarArchive](../../com.aspose.zip/tararchive).

Das folgende Beispiel zeigt, wie man eine Datei komprimiert.

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry(first.bin, \"data.bin\");
archive.save(\"archive.tar\");
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

Dieser Konstruktor entpackt keinen Eintrag. Siehe die Methode [TarEntry.open()](../../com.aspose.zip/tarentry\\#open--) zum Entpacken.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceStream | java.io.InputStream | die Quelle des Archivs |

### TarArchive(String path) {#TarArchive-java.lang.String-}
```
public TarArchive(String path)
```


Initialisiert eine neue Instanz der Klasse [TarArchive](../../com.aspose.zip/tararchive) und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann.

Das folgende Beispiel zeigt, wie man alle Einträge in ein Verzeichnis extrahiert.

```

``````

try (TarArchive archive = new TarArchive(\"archive.tar\")) {
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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Verzeichnis | java.io.File | Verzeichnis zum Komprimieren |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final TarArchive createEntries(File directory, boolean includeRootDirectory)
```


Fügt dem Archiv alle Dateien und Verzeichnisse rekursiv im angegebenen Verzeichnis hinzu.

```

``````

try (FileOutputStream tarFile = new FileOutputStream(\"archive.tar\")) {
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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Quellverzeichnis | java.lang.String | Verzeichnis zum Komprimieren |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntries(String sourceDirectory, boolean includeRootDirectory) {#createEntries-java.lang.String-boolean-}
```
public final TarArchive createEntries(String sourceDirectory, boolean includeRootDirectory)
```


Fügt dem Archiv alle Dateien und Verzeichnisse rekursiv im angegebenen Verzeichnis hinzu.

```

``````

try (FileOutputStream tarFile = new FileOutputStream(\"archive.tar\")) {
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

Der Eintragsname wird ausschließlich über den Parameter `name` festgelegt. Der im Parameter `file` angegebene Dateiname hat keinen Einfluss auf den Eintragsnamen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String | der Name des Eintrags |
| Datei | java.io.File | die Metadaten der Datei oder des Ordners, die komprimiert werden sollen |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, File file, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final TarEntry createEntry(String name, File file, boolean openImmediately)
```


Erstellt einen einzelnen Eintrag im Archiv.

```

``````

File fi = new File(\"data.bin\");
try (TarArchive archive = new TarArchive()) {
archive.createEntry(\"data.bin\", fi);
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

Der Eintragsname wird ausschließlich im Parameter `name` festgelegt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String | der Name des Eintrags |
| source | java.io.InputStream | der Eingabestream für den Eintrag |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, InputStream source, File file) {#createEntry-java.lang.String-java.io.InputStream-java.io.File-}
```
public final TarEntry createEntry(String name, InputStream source, File file)
```


Erstellt einen einzelnen Eintrag im Archiv.

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry(\"bytes\", new ByteArrayInputStream(new byte[] {0x00, (byte) 0xFF}));
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

Der Eintragsname wird ausschließlich im Parameter `name` festgelegt. Der im Parameter `path` angegebene Dateiname beeinflusst den Eintragsnamen nicht.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String | der Name des Eintrags |
| path | java.lang.String | Pfad zur zu komprimierenden Datei |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, String path, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final TarEntry createEntry(String name, String path, boolean openImmediately)
```


Erstellt einen einzelnen Eintrag im Archiv.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| entry | [TarEntry](../../com.aspose.zip/tarentry) | der Eintrag, der aus der Eintragsliste entfernt werden soll |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with the entry deleted
### deleteEntry(int entryIndex) {#deleteEntry-int-}
```
public final TarArchive deleteEntry(int entryIndex)
```


Entfernt den Eintrag aus der Eintragsliste anhand des Index.

```

``````

try (TarArchive archive = new TarArchive(\"two_files.tar\")) {
archive.deleteEntry(0);
archive.save(\"single_file.tar\");
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

Wenn das Verzeichnis nicht existiert, wird es erstellt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| destinationDirectory | java.lang.String | Der Pfad zu dem Verzeichnis, in dem die extrahierten Dateien abgelegt werden sollen |

### fromGZip(InputStream source) {#fromGZip-java.io.InputStream-}
```
public static TarArchive fromGZip(InputStream source)
```


Extrahiert das bereitgestellte gzip-Archiv und erstellt ein [TarArchive](../../com.aspose.zip/tararchive) aus den extrahierten Daten.

Wichtig: Das gzip-Archiv wird in dieser Methode vollständig extrahiert, sein Inhalt wird intern gehalten. Achten Sie auf den Speicherverbrauch.

Der GZip-Extraktionsstrom ist aufgrund des Kompressionsalgorithmus nicht seekbar. Das Tar-Archiv bietet die Möglichkeit, beliebige Datensätze zu extrahieren, daher muss es im Hintergrund mit einem seekbaren Stream arbeiten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| source | java.io.InputStream | die Quelle des Archivs. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromGZip(String path) {#fromGZip-java.lang.String-}
```
public static TarArchive fromGZip(String path)
```


Extrahiert das bereitgestellte gzip-Archiv und erstellt ein [TarArchive](../../com.aspose.zip/tararchive) aus den extrahierten Daten.

Wichtig: Das gzip-Archiv wird in dieser Methode vollständig extrahiert, sein Inhalt wird intern gehalten. Achten Sie auf den Speicherverbrauch.

Der GZip-Extraktionsstrom ist aufgrund des Kompressionsalgorithmus nicht seekbar. Das Tar-Archiv bietet die Möglichkeit, beliebige Datensätze zu extrahieren, daher muss es im Hintergrund mit einem seekbaren Stream arbeiten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | java.lang.String | der Pfad zur Archivdatei. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZ4(InputStream source) {#fromLZ4-java.io.InputStream-}
```
public static TarArchive fromLZ4(InputStream source)
```


Extrahiert das bereitgestellte LZ4-Archiv und erstellt ein [TarArchive](../../com.aspose.zip/tararchive) aus den extrahierten Daten.

Wichtig: Das LZ4-Archiv wird in dieser Methode vollständig extrahiert, sein Inhalt wird intern gehalten. Achten Sie auf den Speicherverbrauch.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | source | java.io.InputStream | Die Quelle des Archivs. |

Der LZ4-Extraktions-Stream ist aufgrund des Kompressionsalgorithmus nicht suchbar. Das Tar-Archiv bietet die Möglichkeit, beliebige Datensätze zu extrahieren, sodass es intern einen suchbaren Stream verwenden muss. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - An instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZ4(String path) {#fromLZ4-java.lang.String-}
```
public static TarArchive fromLZ4(String path)
```


Extrahiert das bereitgestellte LZ4-Archiv und erstellt ein [TarArchive](../../com.aspose.zip/tararchive) aus den extrahierten Daten.

Wichtig: Das LZ4-Archiv wird in dieser Methode vollständig extrahiert, sein Inhalt wird intern gehalten. Achten Sie auf den Speicherverbrauch.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | path | java.lang.String | Der Pfad zur Archivdatei. |

Der LZ4-Extraktions-Stream ist aufgrund des Kompressionsalgorithmus nicht suchbar. Das Tar-Archiv bietet die Möglichkeit, beliebige Datensätze zu extrahieren, sodass es intern einen suchbaren Stream verwenden muss. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - An instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZMA(InputStream source) {#fromLZMA-java.io.InputStream-}
```
public static TarArchive fromLZMA(InputStream source)
```


Extrahiert das bereitgestellte LZMA-Archiv und erstellt ein [TarArchive](../../com.aspose.zip/tararchive) aus den extrahierten Daten.

Wichtig: Das LZMA-Archiv wird in dieser Methode vollständig extrahiert, sein Inhalt wird intern gehalten. Achten Sie auf den Speicherverbrauch.

Der LZMA-Extraktions-Stream ist aufgrund des Kompressionsalgorithmus nicht suchbar. Das Tar-Archiv bietet die Möglichkeit, beliebige Datensätze zu extrahieren, sodass es intern einen suchbaren Stream verwenden muss.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| source | java.io.InputStream | die Quelle des Archivs |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZMA(String path) {#fromLZMA-java.lang.String-}
```
public static TarArchive fromLZMA(String path)
```


Extrahiert das bereitgestellte LZMA-Archiv und erstellt ein [TarArchive](../../com.aspose.zip/tararchive) aus den extrahierten Daten.

Wichtig: Das LZMA-Archiv wird in dieser Methode vollständig extrahiert, sein Inhalt wird intern gehalten. Achten Sie auf den Speicherverbrauch.

Der LZMA-Extraktions-Stream ist aufgrund des Kompressionsalgorithmus nicht suchbar. Das Tar-Archiv bietet die Möglichkeit, beliebige Datensätze zu extrahieren, sodass es intern einen suchbaren Stream verwenden muss.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | java.lang.String | der Pfad zur Archivdatei |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZip(InputStream source) {#fromLZip-java.io.InputStream-}
```
public static TarArchive fromLZip(InputStream source)
```


Extrahiert das bereitgestellte lzip-Archiv und erstellt ein [TarArchive](../../com.aspose.zip/tararchive) aus den extrahierten Daten.

Wichtig: Das lzip-Archiv wird in dieser Methode vollständig extrahiert, sein Inhalt wird intern gehalten. Achten Sie auf den Speicherverbrauch.

Der Lzip-Extraktions-Stream ist aufgrund des Kompressionsalgorithmus nicht suchbar. Das Tar-Archiv bietet die Möglichkeit, beliebige Datensätze zu extrahieren, sodass es intern einen suchbaren Stream verwenden muss

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| source | java.io.InputStream | die Quelle des Archivs. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZip(String path) {#fromLZip-java.lang.String-}
```
public static TarArchive fromLZip(String path)
```


Extrahiert das bereitgestellte lzip-Archiv und erstellt ein [TarArchive](../../com.aspose.zip/tararchive) aus den extrahierten Daten.

Wichtig: Das lzip-Archiv wird in dieser Methode vollständig extrahiert, sein Inhalt wird intern gehalten. Achten Sie auf den Speicherverbrauch.

Der Lzip-Extraktions-Stream ist aufgrund des Kompressionsalgorithmus nicht suchbar. Das Tar-Archiv bietet die Möglichkeit, beliebige Datensätze zu extrahieren, sodass es intern einen suchbaren Stream verwenden muss

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | java.lang.String | der Pfad zur Archivdatei. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromXz(InputStream source) {#fromXz-java.io.InputStream-}
```
public static TarArchive fromXz(InputStream source)
```


Extrahiert das bereitgestellte xz-Format-Archiv und erstellt ein [TarArchive](../../com.aspose.zip/tararchive) aus den extrahierten Daten.

Wichtig: Das xz-Archiv wird in dieser Methode vollständig extrahiert, sein Inhalt wird intern gehalten. Achten Sie auf den Speicherverbrauch.

Das Tar-Archiv bietet die Möglichkeit, beliebige Datensätze zu extrahieren, sodass es intern einen suchbaren Stream verwenden muss.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| source | java.io.InputStream | die Quelle des Archivs |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromXz(String path) {#fromXz-java.lang.String-}
```
public static TarArchive fromXz(String path)
```


Extrahiert das bereitgestellte xz-Format-Archiv und erstellt ein [TarArchive](../../com.aspose.zip/tararchive) aus den extrahierten Daten.

Wichtig: Das xz-Archiv wird in dieser Methode vollständig extrahiert, sein Inhalt wird intern gehalten. Achten Sie auf den Speicherverbrauch.

Das Tar-Archiv bietet die Möglichkeit, beliebige Datensätze zu extrahieren, sodass es intern einen suchbaren Stream verwenden muss.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | java.lang.String | der Pfad zur Archivdatei |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZ(InputStream source) {#fromZ-java.io.InputStream-}
```
public static TarArchive fromZ(InputStream source)
```


Extrahiert das bereitgestellte Z-Format-Archiv und erstellt ein [TarArchive](../../com.aspose.zip/tararchive) aus den extrahierten Daten.

Wichtig: Das Z-Archiv wird in dieser Methode vollständig extrahiert, sein Inhalt wird intern gehalten. Achten Sie auf den Speicherverbrauch.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| source | java.io.InputStream | die Quelle des Archivs |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZ(String path) {#fromZ-java.lang.String-}
```
public static TarArchive fromZ(String path)
```


Extrahiert das bereitgestellte Z-Format-Archiv und erstellt ein [TarArchive](../../com.aspose.zip/tararchive) aus den extrahierten Daten.

Wichtig: Das Z-Archiv wird in dieser Methode vollständig extrahiert, sein Inhalt wird intern gehalten. Achten Sie auf den Speicherverbrauch.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | java.lang.String | der Pfad zur Archivdatei |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZstandard(InputStream source) {#fromZstandard-java.io.InputStream-}
```
public static TarArchive fromZstandard(InputStream source)
```


Extrahiert das bereitgestellte Zstandard-Archiv und erstellt ein [TarArchive](../../com.aspose.zip/tararchive) aus den extrahierten Daten.

Wichtig: Das Zstandard-Archiv wird in dieser Methode vollständig extrahiert, sein Inhalt wird intern gehalten. Achten Sie auf den Speicherverbrauch.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| source | java.io.InputStream | die Quelle des Archivs |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZstandard(String path) {#fromZstandard-java.lang.String-}
```
public static TarArchive fromZstandard(String path)
```


Extrahiert das bereitgestellte Zstandard-Archiv und erstellt ein [TarArchive](../../com.aspose.zip/tararchive) aus den extrahierten Daten.

Wichtig: Das Zstandard-Archiv wird in dieser Methode vollständig extrahiert, sein Inhalt wird intern gehalten. Achten Sie auf den Speicherverbrauch.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | java.lang.String | der Pfad zur Archivdatei |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### getEntries() {#getEntries--}
```
public final List<TarEntry> getEntries()
```


Ruft Einträge des Typs [TarEntry](../../com.aspose.zip/tarentry) ab, die das Archiv bilden.

**Returns:**
java.util.List&lt;com.aspose.zip.TarEntry&gt; - Einträge des Typs [TarEntry](../../com.aspose.zip/tarentry), die das Archiv bilden
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Ruft Einträge des Typs [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) ab, die das Tar-Archiv bilden.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - Einträge des Typs [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), die das Tar-Archiv bilden
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Liefert das Archivformat.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Speichert das Archiv in den angegebenen Stream.

```

``````

try (FileOutputStream tarFile = new FileOutputStream(\"archive.tar\")) {
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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Ausgabe | java.io.OutputStream | Ziel-Stream. |

`output` muss beschreibbar sein |
| format | [TarFormat](../../com.aspose.zip/tarformat) | definiert das Tar-Header-Format. Null-Werte werden, wenn möglich, als USTar behandelt |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Speichert das Archiv in die angegebene Zieldatei.

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

Es ist möglich, ein Archiv am selben Pfad zu speichern, von dem es geladen wurde. Dies wird jedoch nicht empfohlen, da dieser Ansatz das Kopieren in eine temporäre Datei verwendet.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| destinationFileName | java.lang.String | Der Pfad des zu erstellenden Archivs. Wenn der angegebene Dateiname auf eine bereits vorhandene Datei verweist, wird diese überschrieben. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | definiert das Tar-Header-Format. Null-Werte werden, wenn möglich, als USTar behandelt |

### saveGzipped(OutputStream output) {#saveGzipped-java.io.OutputStream-}
```
public final void saveGzipped(OutputStream output)
```


Speichert das Archiv in den Stream mit gzip-Kompression.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Ausgabe | java.io.OutputStream | Ziel-Stream. |

`output` muss beschreibbar sein |
| format | [TarFormat](../../com.aspose.zip/tarformat) | definiert das Tar-Header-Format. Null-Werte werden, wenn möglich, als USTar behandelt |

### saveGzipped(String path) {#saveGzipped-java.lang.String-}
```
public final void saveGzipped(String path)
```


Speichert das Archiv in die Datei über den Pfad mit gzip-Kompression.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | java.lang.String | der Pfad des zu erstellenden Archivs. Wenn der angegebene Dateiname auf eine bereits vorhandene Datei verweist, wird sie überschrieben |
| format | [TarFormat](../../com.aspose.zip/tarformat) | definiert das Tar-Header-Format. Null-Werte werden, wenn möglich, als USTar behandelt |

### saveLZ4Compressed(OutputStream output) {#saveLZ4Compressed-java.io.OutputStream-}
```
public final void saveLZ4Compressed(OutputStream output)
```


Speichert das Archiv im Stream mit LZ4-Kompression.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Ausgabe | java.io.OutputStream | Ziel-Stream. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | Definiert das Tar-Header-Format. Null-Werte werden, wenn möglich, als USTar behandelt. |

### saveLZ4Compressed(String path) {#saveLZ4Compressed-java.lang.String-}
```
public final void saveLZ4Compressed(String path)
```


Speichert das Archiv in die Datei über den Pfad mit LZ4-Kompression.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | java.lang.String | Der Pfad des zu erstellenden Archivs. Wenn der angegebene Dateiname auf eine bereits vorhandene Datei zeigt, wird diese überschrieben. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | Definiert das Tar-Header-Format. Null-Werte werden, wenn möglich, als USTar behandelt. |

### saveLZMACompressed(OutputStream output) {#saveLZMACompressed-java.io.OutputStream-}
```
public final void saveLZMACompressed(OutputStream output)
```


Speichert das Archiv im Stream mit LZMA-Kompression.

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

Wichtig: Das tar-Archiv wird in dieser Methode zuerst erstellt und dann komprimiert, sein Inhalt wird intern gespeichert. Achtung bei der Speichernutzung.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Ausgabe | java.io.OutputStream | Ziel-Stream. |

`output` muss beschreibbar sein |
| format | [TarFormat](../../com.aspose.zip/tarformat) | definiert das Tar-Header-Format. Null-Werte werden, wenn möglich, als USTar behandelt |

### saveLZMACompressed(String path) {#saveLZMACompressed-java.lang.String-}
```
public final void saveLZMACompressed(String path)
```


Speichert das Archiv in die Datei über den Pfad mit lzma-Kompression.

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

Wichtig: Das tar-Archiv wird in dieser Methode zuerst erstellt und dann komprimiert, sein Inhalt wird intern gespeichert. Achtung bei der Speichernutzung.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | java.lang.String | der Pfad des zu erstellenden Archivs. Wenn der angegebene Dateiname auf eine bereits vorhandene Datei verweist, wird sie überschrieben |
| format | [TarFormat](../../com.aspose.zip/tarformat) | definiert das Tar-Header-Format. Null-Werte werden, wenn möglich, als USTar behandelt |

### saveLzipped(OutputStream output) {#saveLzipped-java.io.OutputStream-}
```
public final void saveLzipped(OutputStream output)
```


Speichert das Archiv in den Stream mit lzip-Kompression.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Ausgabe | java.io.OutputStream | Ziel-Stream. |

`output` muss beschreibbar sein |
| format | [TarFormat](../../com.aspose.zip/tarformat) | definiert das Tar-Header-Format. Null-Werte werden, wenn möglich, als USTar behandelt |

### saveLzipped(String path) {#saveLzipped-java.lang.String-}
```
public final void saveLzipped(String path)
```


Speichert das Archiv in die Datei über den Pfad mit lzip-Kompression.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | java.lang.String | der Pfad des zu erstellenden Archivs. Wenn der angegebene Dateiname auf eine bereits vorhandene Datei verweist, wird sie überschrieben |
| format | [TarFormat](../../com.aspose.zip/tarformat) | definiert das Tar-Header-Format. Null-Werte werden, wenn möglich, als USTar behandelt |

### saveXzCompressed(OutputStream output) {#saveXzCompressed-java.io.OutputStream-}
```
public final void saveXzCompressed(OutputStream output)
```


Speichert das Archiv in den Stream mit xz-Kompression.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Ausgabe | java.io.OutputStream | Ziel-Stream. |

`output`Der Stream muss beschreibbar sein |
| format | [TarFormat](../../com.aspose.zip/tarformat) | definiert das Tar-Header-Format. Null-Werte werden, wenn möglich, als USTar behandelt |

### saveXzCompressed(OutputStream output, TarFormat format, XzArchiveSettings settings) {#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-}
```
public final void saveXzCompressed(OutputStream output, TarFormat format, XzArchiveSettings settings)
```


Speichert das Archiv in den Stream mit xz-Kompression.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | java.lang.String | der Pfad des zu erstellenden Archivs. Wenn der angegebene Dateiname auf eine bereits vorhandene Datei verweist, wird sie überschrieben |

### saveXzCompressed(String path, TarFormat format) {#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveXzCompressed(String path, TarFormat format)
```


Speichert das Archiv in die Datei über den Pfad mit xz-Kompression.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | java.lang.String | der Pfad des zu erstellenden Archivs. Wenn der angegebene Dateiname auf eine bereits vorhandene Datei verweist, wird sie überschrieben |
| format | [TarFormat](../../com.aspose.zip/tarformat) | definiert das Tar-Header-Format. Null-Werte werden, wenn möglich, als USTar behandelt |
| settings | [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) | Satz von Einstellungen für ein bestimmtes xz-Archiv: Wörterbuchgröße, Blockgröße, Prüftyp |

### saveZCompressed(OutputStream output) {#saveZCompressed-java.io.OutputStream-}
```
public final void saveZCompressed(OutputStream output)
```


Speichert das Archiv in den Stream mit Z-Kompression.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Ausgabe | java.io.OutputStream | der Ziel-Stream |
| format | [TarFormat](../../com.aspose.zip/tarformat) | definiert das Tar-Header-Format. Null-Werte werden, wenn möglich, als USTar behandelt |

### saveZCompressed(String path) {#saveZCompressed-java.lang.String-}
```
public final void saveZCompressed(String path)
```


Speichert das Archiv in die Datei über den Pfad mit Z-Kompression.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | java.lang.String | der Pfad des zu erstellenden Archivs. Wenn der angegebene Dateiname auf eine bereits vorhandene Datei verweist, wird sie überschrieben |
| format | [TarFormat](../../com.aspose.zip/tarformat) | definiert das Tar-Header-Format. Null-Werte werden, wenn möglich, als USTar behandelt |

### saveZstandard(OutputStream output) {#saveZstandard-java.io.OutputStream-}
```
public final void saveZstandard(OutputStream output)
```


Speichert das Archiv in den Stream mit Zstandard-Kompression.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Ausgabe | java.io.OutputStream | Ziel-Stream. |

`output` muss beschreibbar sein |
| format | [TarFormat](../../com.aspose.zip/tarformat) | definiert das Tar-Header-Format. Null-Werte werden, wenn möglich, als USTar behandelt |

### saveZstandard(String path) {#saveZstandard-java.lang.String-}
```
public final void saveZstandard(String path)
```


Speichert das Archiv in die Datei über den Pfad mit Zstandard-Kompression.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | java.lang.String | der Pfad des zu erstellenden Archivs. Wenn der angegebene Dateiname auf eine bereits vorhandene Datei verweist, wird sie überschrieben |
| format | [TarFormat](../../com.aspose.zip/tarformat) | definiert das Tar-Header-Format. Null-Werte werden, wenn möglich, als USTar behandelt |

