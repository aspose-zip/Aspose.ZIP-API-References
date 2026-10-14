---
title: "Bzip2Archive"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Diese Klasse repräsentiert eine bzip2-Archivdatei."
type: docs
weight: 40
url: /de/java/com.aspose.zip/bzip2archive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class Bzip2Archive implements IArchive, IArchiveFileEntry, AutoCloseable
```

Diese Klasse stellt eine bzip2-Archivdatei dar. Verwenden Sie sie zum Erstellen oder Extrahieren von bzip2-Archiven.

bzip2 komprimiert Dateien mit dem Burrows-Wheeler-Blocksortier-Textkompressionsalgorithmus und Huffman-Codierung. Mehr dazu: [Bzip2][]


[Bzip2]: https://en.wikipedia.org/wiki/Bzip2
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [Bzip2Archive()](#Bzip2Archive--) | Initialisiert eine neue Instanz der Klasse [Bzip2Archive](../../com.aspose.zip/bzip2archive) zum Komprimieren. |
| [Bzip2Archive(InputStream sourceStream)](#Bzip2Archive-java.io.InputStream-) | Initialisiert eine neue Instanz der Klasse [Bzip2Archive](../../com.aspose.zip/bzip2archive) zum Dekomprimieren. |
| [Bzip2Archive(InputStream sourceStream, Bzip2LoadOptions loadOptions)](#Bzip2Archive-java.io.InputStream-com.aspose.zip.Bzip2LoadOptions-) | Initialisiert eine neue Instanz der Klasse [Bzip2Archive](../../com.aspose.zip/bzip2archive) zum Dekomprimieren. |
| [Bzip2Archive(String path)](#Bzip2Archive-java.lang.String-) | Initialisiert eine neue Instanz der Klasse [Bzip2Archive](../../com.aspose.zip/bzip2archive) zum Dekomprimieren. |
| [Bzip2Archive(String path, Bzip2LoadOptions loadOptions)](#Bzip2Archive-java.lang.String-com.aspose.zip.Bzip2LoadOptions-) | Initialisiert eine neue Instanz der Klasse [Bzip2Archive](../../com.aspose.zip/bzip2archive) zum Dekomprimieren. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrahiert das Archiv in den bereitgestellten Stream. |
| [extract(String path)](#extract-java.lang.String-) | Extrahiert das Archiv in die Datei anhand des Pfads. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrahiert den Inhalt des Archivs in das angegebene Verzeichnis. |
| [getFileEntries()](#getFileEntries--) | Liefert Einträge des Typs [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), die das bzip2-Archiv bilden. |
| [getFormat()](#getFormat--) | Liefert das Archivformat. |
| [getLength()](#getLength--) | Liefert die Länge. |
| [getName()](#getName--) | Der Name der Originaldatei. |
| [open()](#open--) | Öffnet das Archiv zum Extrahieren und stellt einen Stream mit dem Archivinhalt bereit. |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | Speichert das Archiv in den angegebenen Stream. |
| [save(OutputStream outputStream, Bzip2SaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.Bzip2SaveOptions-) | Speichert das Archiv in den angegebenen Stream. |
| [save(String destinationFileName)](#save-java.lang.String-) | Speichert das Archiv in die angegebene Zieldatei. |
| [save(String destinationFileName, Bzip2SaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.Bzip2SaveOptions-) | Speichert das Archiv in die angegebene Zieldatei. |
| [setSource(CpioArchive cpioArchive)](#setSource-com.aspose.zip.CpioArchive-) | Legt den Inhalt fest, der im Archiv komprimiert werden soll. |
| [setSource(CpioArchive cpioArchive, CpioFormat format)](#setSource-com.aspose.zip.CpioArchive-com.aspose.zip.CpioFormat-) | Legt den Inhalt fest, der im Archiv komprimiert werden soll. |
| [setSource(TarArchive tarArchive)](#setSource-com.aspose.zip.TarArchive-) | Legt den Inhalt fest, der im Archiv komprimiert werden soll. |
| [setSource(TarArchive tarArchive, TarFormat format)](#setSource-com.aspose.zip.TarArchive-com.aspose.zip.TarFormat-) | Legt den Inhalt fest, der im Archiv komprimiert werden soll. |
| [setSource(File file)](#setSource-java.io.File-) | Legt den Inhalt fest, der im Archiv komprimiert werden soll. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Legt den Inhalt fest, der im Archiv komprimiert werden soll. |
| [setSource(String path)](#setSource-java.lang.String-) | Legt den Inhalt fest, der im Archiv komprimiert werden soll. |
### Bzip2Archive() {#Bzip2Archive--}
```
public Bzip2Archive()
```


Initialisiert eine neue Instanz der Klasse [Bzip2Archive](../../com.aspose.zip/bzip2archive) zum Komprimieren.

Das folgende Beispiel zeigt, wie man eine Datei komprimiert.

```

``````

try (Bzip2Archive archive = new Bzip2Archive()) {
archive.setSource("data.bin");
archive.save("archive.bz2");
}
 
```



### Bzip2Archive(InputStream sourceStream) {#Bzip2Archive-java.io.InputStream-}
```
public Bzip2Archive(InputStream sourceStream)
```


Initializes a new instance of the [Bzip2Archive](../../com.aspose.zip/bzip2archive) class prepared for decompressing.

Open an archive from a stream and extract it to a `ByteArrayOutputStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (Bzip2Archive archive = new Bzip2Archive(new FileInputStream("archive.bz2"))) {
         InputStream decompressed = archive.open();
         byte[] b = new byte[8192];
         int bytesRead;
         while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

Dieser Konstruktor dekomprimiert nicht. Siehe die Methode [open()](../../com.aspose.zip/bzip2archive\#open--) zum Dekomprimieren.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceStream | java.io.InputStream | die Quelle des Archivs |

### Bzip2Archive(InputStream sourceStream, Bzip2LoadOptions loadOptions) {#Bzip2Archive-java.io.InputStream-com.aspose.zip.Bzip2LoadOptions-}
```
public Bzip2Archive(InputStream sourceStream, Bzip2LoadOptions loadOptions)
```


Initialisiert eine neue Instanz der Klasse [Bzip2Archive](../../com.aspose.zip/bzip2archive) zum Dekomprimieren.

Öffnen Sie ein Archiv aus einem Stream und extrahieren Sie es in einen `ByteArrayOutputStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (Bzip2Archive archive = new Bzip2Archive(new FileInputStream("archive.bz2"))) {
InputStream decompressed = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/bzip2archive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |
| loadOptions | [Bzip2LoadOptions](../../com.aspose.zip/bzip2loadoptions) | the options to load archive with |

### Bzip2Archive(String path) {#Bzip2Archive-java.lang.String-}
```
public Bzip2Archive(String path)
```


Initializes a new instance of the [Bzip2Archive](../../com.aspose.zip/bzip2archive) class prepared for decompressing.

Open an archive from file by path and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (Bzip2Archive archive = new Bzip2Archive("archive.bz2")) {
         InputStream decompressed = archive.open();
         byte[] b = new byte[8192];
         int bytesRead;
         while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

Dieser Konstruktor dekomprimiert nicht. Siehe die Methode [open()](../../com.aspose.zip/bzip2archive\#open--) zum Dekomprimieren.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | java.lang.String | der Pfad zur Archivdatei |

### Bzip2Archive(String path, Bzip2LoadOptions loadOptions) {#Bzip2Archive-java.lang.String-com.aspose.zip.Bzip2LoadOptions-}
```
public Bzip2Archive(String path, Bzip2LoadOptions loadOptions)
```


Initialisiert eine neue Instanz der Klasse [Bzip2Archive](../../com.aspose.zip/bzip2archive) zum Dekomprimieren.

Öffnen Sie ein Archiv aus einer Datei über den Pfad und extrahieren Sie es in einen `MemoryStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (Bzip2Archive archive = new Bzip2Archive("archive.bz2")) {
InputStream decompressed = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/bzip2archive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |
| loadOptions | [Bzip2LoadOptions](../../com.aspose.zip/bzip2loadoptions) | the options to load archive with |

### close() {#close--}
```
public void close()
```




### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts the archive to the stream provided.

```

``````

     try (Bzip2Archive archive = new Bzip2Archive("archive.bz2")) {
         archive.extract(httpResponseStream);
     }
 
```



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Ziel | java.io.OutputStream | Ziel-Stream. Muss beschreibbar sein. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extrahiert das Archiv in die Datei anhand des Pfads.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | java.lang.String | Der Pfad zur Zieldatei. Wenn die Datei bereits existiert, wird sie überschrieben. |

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
|  | destinationDirectory | java.lang.String | Der Pfad zum Verzeichnis, in dem die extrahierten Dateien abgelegt werden sollen. |

Wenn das Verzeichnis nicht existiert, wird es erstellt. |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Liefert Einträge des Typs [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), die das bzip2-Archiv bilden.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - Einträge des Typs [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), die das bzip2-Archiv bilden
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
### open() {#open--}
```
public final InputStream open()
```


Öffnet das Archiv zum Extrahieren und stellt einen Stream mit dem Archivinhalt bereit.


Verwendung:

```

``````

try (InputStream decompressed = archive.open()) {
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
fileStream.write(buffer, 0, bytesRead);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

Read from the stream to get the original content of the file. See examples section.

**Returns:**
java.io.InputStream - the stream that represents the contents of the archive
### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


Saves archive to the stream provided.

Write compressed data to an output stream.

```

``````

     try (Bzip2Archive archive = new Bzip2Archive()) {
         archive.setSource(new File("data.bin"));
         archive.save(outputStream);
     }
 
```



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| outputStream | java.io.OutputStream | Ziel-Stream. |

### save(OutputStream outputStream, Bzip2SaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.Bzip2SaveOptions-}
```
public final void save(OutputStream outputStream, Bzip2SaveOptions saveOptions)
```


Speichert das Archiv in den angegebenen Stream.

Komprimierte Daten in einen Ausgabestream schreiben.

```

``````

try (Bzip2Archive archive = new Bzip2Archive()) {
archive.setSource(new File("data.bin"));
archive.save(outputStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outputStream | java.io.OutputStream | destination stream. |
| saveOptions | [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions) | options for saving a bzip2 archive. If not specified, 900 Kb block size would be used |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves archive to the destination file provided.

Writes compressed data to file.

```

``````

     try (Bzip2Archive archive = new Bzip2Archive()) {
         archive.setSource(new File("data.bin"));
         archive.save("data.bz2");
     }
 
```



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| destinationFileName | java.lang.String | der Pfad des zu erstellenden Archivs. Wenn der angegebene Dateiname auf eine bereits vorhandene Datei verweist, wird sie überschrieben |

### save(String destinationFileName, Bzip2SaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.Bzip2SaveOptions-}
```
public final void save(String destinationFileName, Bzip2SaveOptions saveOptions)
```


Speichert das Archiv in die angegebene Zieldatei.

Schreibt komprimierte Daten in eine Datei.

```

``````

try (Bzip2Archive archive = new Bzip2Archive()) {
archive.setSource(new File("data.bin"));
archive.save("data.bz2");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| saveOptions | [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions) | options for saving a bzip2 archive. If not specified, 900 Kb block size would be used |

### setSource(CpioArchive cpioArchive) {#setSource-com.aspose.zip.CpioArchive-}
```
public final void setSource(CpioArchive cpioArchive)
```


Sets the content to be compressed within the archive.

```

``````

     try (CpioArchive cpioArchive = new CpioArchive()) {
         cpioArchive.createEntry("first.bin", "data1.bin");
         cpioArchive.createEntry("second.bin", "data2.bin");
         try (Bzip2Archive bzippedArchive = new Bzip2Archive()) {
             bzippedArchive.setSource(cpioArchive);
             bzippedArchive.save("archive.cpio.bz2");
         }
     }
 
```

Verwenden Sie diese Methode, um ein gemeinsames cpio.bz2-Archiv zu erstellen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cpioArchive | [CpioArchive](../../com.aspose.zip/cpioarchive) | cpio-Archiv, das komprimiert werden soll |

### setSource(CpioArchive cpioArchive, CpioFormat format) {#setSource-com.aspose.zip.CpioArchive-com.aspose.zip.CpioFormat-}
```
public final void setSource(CpioArchive cpioArchive, CpioFormat format)
```


Legt den Inhalt fest, der im Archiv komprimiert werden soll.

```

``````

try (CpioArchive cpioArchive = new CpioArchive()) {
cpioArchive.createEntry("first.bin", "data1.bin");
cpioArchive.createEntry("second.bin", "data2.bin");
try (Bzip2Archive bzippedArchive = new Bzip2Archive()) {
bzippedArchive.setSource(cpioArchive);
bzippedArchive.save("archive.cpio.bz2");
}
}
 
```

Use this method to compose joint cpio.bz2 archive.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cpioArchive | [CpioArchive](../../com.aspose.zip/cpioarchive) | cpio archive to be compressed |
| format | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### setSource(TarArchive tarArchive) {#setSource-com.aspose.zip.TarArchive-}
```
public final void setSource(TarArchive tarArchive)
```


Sets the content to be compressed within the archive.

```

``````

     try (TarArchive tarArchive = new TarArchive()) {
         tarArchive.createEntry("first.bin", "data1.bin");
         tarArchive.createEntry("second.bin", "data2.bin");
         try (Bzip2Archive bzippedArchive = new Bzip2Archive()) {
             bzippedArchive.setSource(tarArchive);
             bzippedArchive.save("archive.tar.bz2");
         }
     }
 
```

Verwenden Sie diese Methode, um ein gemeinsames tar.bz2-Archiv zu erstellen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| tarArchive | [TarArchive](../../com.aspose.zip/tararchive) | tar-Archiv, das komprimiert werden soll |

### setSource(TarArchive tarArchive, TarFormat format) {#setSource-com.aspose.zip.TarArchive-com.aspose.zip.TarFormat-}
```
public final void setSource(TarArchive tarArchive, TarFormat format)
```


Legt den Inhalt fest, der im Archiv komprimiert werden soll.

```

``````

try (TarArchive tarArchive = new TarArchive()) {
tarArchive.createEntry("first.bin", "data1.bin");
tarArchive.createEntry("second.bin", "data2.bin");
try (Bzip2Archive bzippedArchive = new Bzip2Archive()) {
bzippedArchive.setSource(tarArchive);
bzippedArchive.save("archive.tar.bz2");
}
}
 
```

Use this method to compose joint tar.bz2 archive.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| tarArchive | [TarArchive](../../com.aspose.zip/tararchive) | tar archive to be compressed |
| format | [TarFormat](../../com.aspose.zip/tarformat) | defines tar header format |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Sets the content to be compressed within the archive.

```

``````

     try (Bzip2Archive archive = new Bzip2Archive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.bz2");
     }
 
```



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Datei | java.io.File | die Referenz zu einer zu komprimierenden Datei |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Legt den Inhalt fest, der im Archiv komprimiert werden soll.

```

``````

try (Bzip2Archive archive = new Bzip2Archive()) {
archive.setSource(new ByteArrayInputStream(new byte[] { 0x00, (byte) 0xFF }));
archive.save("archive.bz2");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | the input stream for the archive |

### setSource(String path) {#setSource-java.lang.String-}
```
public final void setSource(String path)
```


Sets the content to be compressed within the archive.

```

``````

     try (Bzip2Archive archive = new Bzip2Archive()) {
         archive.setSource("data.bin");
         archive.save("archive.bz2");
     }
 
```



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | java.lang.String | Pfad zur zu komprimierenden Datei |

