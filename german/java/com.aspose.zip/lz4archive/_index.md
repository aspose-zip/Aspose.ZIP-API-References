---
title: "Lz4Archive"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Diese Klasse stellt eine LZ4-Archivdatei dar."
type: docs
weight: 80
url: /de/java/com.aspose.zip/lz4archive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class Lz4Archive implements IArchive, IArchiveFileEntry, AutoCloseable
```

Diese Klasse repräsentiert eine LZ4-Archivdatei. Verwenden Sie sie, um LZ4-Archive zu extrahieren oder zu erstellen.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [Lz4Archive(InputStream sourceStream)](#Lz4Archive-java.io.InputStream-) | Initialisiert eine neue Instanz der [Lz4Archive](../../com.aspose.zip/lz4archive)-Klasse, die für das Dekomprimieren vorbereitet ist. |
| [Lz4Archive(InputStream sourceStream, Lz4LoadOptions loadOptions)](#Lz4Archive-java.io.InputStream-com.aspose.zip.Lz4LoadOptions-) | Initialisiert eine neue Instanz der [Lz4Archive](../../com.aspose.zip/lz4archive)-Klasse, die für das Dekomprimieren vorbereitet ist. |
| [Lz4Archive(String path)](#Lz4Archive-java.lang.String-) | Initialisiert eine neue Instanz der [Lz4Archive](../../com.aspose.zip/lz4archive)-Klasse. |
| [Lz4Archive(String path, Lz4LoadOptions loadOptions)](#Lz4Archive-java.lang.String-com.aspose.zip.Lz4LoadOptions-) | Initialisiert eine neue Instanz der [Lz4Archive](../../com.aspose.zip/lz4archive)-Klasse. |
| [Lz4Archive()](#Lz4Archive--) | Initialisiert eine neue Instanz der [Lz4Archive](../../com.aspose.zip/lz4archive)-Klasse, die für das Komprimieren vorbereitet ist. |
| [Lz4Archive(Lz4ArchiveSetting settings)](#Lz4Archive-com.aspose.zip.Lz4ArchiveSetting-) | Initialisiert eine neue Instanz der [Lz4Archive](../../com.aspose.zip/lz4archive)-Klasse, die für das Komprimieren vorbereitet ist. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrahiert das Archiv in den bereitgestellten Stream. |
| [extract(String path)](#extract-java.lang.String-) | Extrahiert das Archiv in die Datei anhand des Pfads. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrahiert den Inhalt des Archivs in das angegebene Verzeichnis. |
| [getFileEntries()](#getFileEntries--) | Ruft Einträge vom Typ [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) ab, die das Archiv bilden. |
| [getFormat()](#getFormat--) | Liefert das Archivformat. |
| [getLength()](#getLength--) | Liefert die Länge. |
| [getName()](#getName--) | Liefert den Originalnamen. |
| [open()](#open--) | Öffnet das Archiv zum Extrahieren und stellt einen Stream mit dem Archivinhalt bereit. |
| [save(File destination)](#save-java.io.File-) | Speichert das LZ4-Archiv in die angegebene Zieldatei. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Speichert das LZ4-Archiv in den bereitgestellten Stream. |
| [save(String destinationFileName)](#save-java.lang.String-) | Speichert das Archiv in die angegebene Zieldatei. |
| [setSource(TarArchive tarArchive)](#setSource-com.aspose.zip.TarArchive-) | Legt den Inhalt fest, der im Archiv komprimiert werden soll. |
| [setSource(TarArchive tarArchive, TarFormat format)](#setSource-com.aspose.zip.TarArchive-com.aspose.zip.TarFormat-) | Legt den Inhalt fest, der im Archiv komprimiert werden soll. |
| [setSource(File fileInfo)](#setSource-java.io.File-) | Legt den Inhalt fest, der im Archiv komprimiert werden soll. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Legt den Inhalt fest, der im Archiv komprimiert werden soll. |
| [setSource(String path)](#setSource-java.lang.String-) | Legt den Inhalt fest, der im Archiv komprimiert werden soll. |
### Lz4Archive(InputStream sourceStream) {#Lz4Archive-java.io.InputStream-}
```
public Lz4Archive(InputStream sourceStream)
```


Initialisiert eine neue Instanz der [Lz4Archive](../../com.aspose.zip/lz4archive)-Klasse, die für das Dekomprimieren vorbereitet ist.

Öffnet ein Archiv aus einem Stream und extrahiert es in einen `MemoryStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (Lz4Archive archive = new Lz4Archive(new FileInputStream(\"archive.lz4\"))) {
InputStream decompressed = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/lz4archive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |

### Lz4Archive(InputStream sourceStream, Lz4LoadOptions loadOptions) {#Lz4Archive-java.io.InputStream-com.aspose.zip.Lz4LoadOptions-}
```
public Lz4Archive(InputStream sourceStream, Lz4LoadOptions loadOptions)
```


Initializes a new instance of the [Lz4Archive](../../com.aspose.zip/lz4archive) class prepared for decompressing.

Open an archive from a stream and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (Lz4Archive archive = new Lz4Archive(new FileInputStream("archive.lz4"))) {
         InputStream decompressed = archive.open();
         byte[] b = new byte[8192];
         int bytesRead;
         while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
     }
 
```

Dieser Konstruktor dekomprimiert nicht. Siehe die Methode [open()](../../com.aspose.zip/lz4archive\\#open--) zum Dekomprimieren.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceStream | java.io.InputStream | die Quelle des Archivs |
| loadOptions | [Lz4LoadOptions](../../com.aspose.zip/lz4loadoptions) | Die Optionen, mit denen das Archiv geladen wird. |

### Lz4Archive(String path) {#Lz4Archive-java.lang.String-}
```
public Lz4Archive(String path)
```


Initialisiert eine neue Instanz der [Lz4Archive](../../com.aspose.zip/lz4archive)-Klasse.

Öffnen Sie ein Archiv aus einer Datei über den Pfad und extrahieren Sie es in einen `MemoryStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (Lz4Archive archive = new Lz4Archive(\"archive.lz4\")) {
InputStream decompressed = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/lz4archive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### Lz4Archive(String path, Lz4LoadOptions loadOptions) {#Lz4Archive-java.lang.String-com.aspose.zip.Lz4LoadOptions-}
```
public Lz4Archive(String path, Lz4LoadOptions loadOptions)
```


Initializes a new instance of the [Lz4Archive](../../com.aspose.zip/lz4archive) class.

Open an archive from file by path and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (Lz4Archive archive = new Lz4Archive("archive.lz4")) {
         InputStream decompressed = archive.open();
         byte[] b = new byte[8192];
         int bytesRead;
         while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
     }
 
```

Dieser Konstruktor dekomprimiert nicht. Siehe die Methode [open()](../../com.aspose.zip/lz4archive\\#open--) zum Dekomprimieren.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | java.lang.String | der Pfad zur Archivdatei |
| loadOptions | [Lz4LoadOptions](../../com.aspose.zip/lz4loadoptions) | Die Optionen, mit denen das Archiv geladen wird. |

### Lz4Archive() {#Lz4Archive--}
```
public Lz4Archive()
```


Initialisiert eine neue Instanz der [Lz4Archive](../../com.aspose.zip/lz4archive)-Klasse, die für das Komprimieren vorbereitet ist.

### Lz4Archive(Lz4ArchiveSetting settings) {#Lz4Archive-com.aspose.zip.Lz4ArchiveSetting-}
```
public Lz4Archive(Lz4ArchiveSetting settings)
```


Initialisiert eine neue Instanz der [Lz4Archive](../../com.aspose.zip/lz4archive)-Klasse, die für das Komprimieren vorbereitet ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| settings | [Lz4ArchiveSetting](../../com.aspose.zip/lz4archivesetting) | Die Einstellung des zusammengesetzten Archivs. |

### close() {#close--}
```
public void close()
```




### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extrahiert das Archiv in den bereitgestellten Stream.

```

``````

OutputStream httpResponseStream = null;
try (Lz4Archive archive = new Lz4Archive(\"archive.lz4\")) {
archive.extract(httpResponseStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the archive to the file by path.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to destination file. If the file already exists, it will be overwritten |

**Returns:**
java.io.File - info of an extracted file
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts content of the archive to the directory provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in. If the directory does not exist, it will be created |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the archive
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


Gets the original name.

**Returns:**
java.lang.String - the original name
### open() {#open--}
```
public final InputStream open()
```


Opens the archive for extraction and provides a stream with archive content.

Extracts the archive and copies extracted content to file stream.

```

``````

     try (Lz4Archive archive = new Lz4Archive("archive.lz4")) {
         try (FileOutputStream extracted = new FileOutputStream("data.bin")) {
             InputStream unpacked = archive.open();
             byte[] b = new byte[8192];
             int bytesRead;
             while (0 < (bytesRead = unpacked.read(b, 0, b.length))) {
                 extracted.write(b, 0, bytesRead);
             }
         }
     } catch (IOException ex) {
     }
 
```

Lesen Sie aus dem Stream, um den ursprünglichen Inhalt einer Datei zu erhalten. Siehe den Abschnitt Beispiele.

**Returns:**
java.io.InputStream – der Stream, der den Inhalt des Archivs darstellt
### save(File destination) {#save-java.io.File-}
```
public final void save(File destination)
```


Speichert das LZ4-Archiv in die angegebene Zieldatei.

```

``````

try (Lz4Archive archive = new Lz4Archive()) {
archive.setSource(new File("data.bin"));
archive.save(new File(\"archive.lz4\"));
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.File | File, which will be opened as destination stream. |

### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves lz4 archive to the stream provided.

```

``````

     try (FileOutputStream lz4File = new FileOutputStream("archive.lz4")) {
         try (Lz4Archive archive = new Lz4Archive()) {
             archive.setSource("data.bin");
             archive.save(lz4File);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Ausgabe | java.io.OutputStream | Ziel-Stream. |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Speichert das Archiv in die angegebene Zieldatei.

```

``````

try (Lz4Archive archive = new Lz4Archive()) {
archive.setSource("data.bin");
archive.save(\"archive.lz4\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |

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
         try (Lz4Archive lz4Archive = new Lz4Archive()) {
             lz4Archive.setSource(tarArchive);
             lz4Archive.save("archive.tar.lz4");
         }
     }
 
```

Verwenden Sie diese Methode, um ein gemeinsames tar.lz4-Archiv zu erstellen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| tarArchive | [TarArchive](../../com.aspose.zip/tararchive) | Tar-Archiv, das komprimiert werden soll. |

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
try (Lz4Archive lz4Archive = new Lz4Archive()) {
lz4Archive.setSource(tarArchive);
lz4Archive.save("archive.tar.lz4");
}
}
 
```

Use this method to compose joint tar.lz4 archive.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| tarArchive | [TarArchive](../../com.aspose.zip/tararchive) | Tar archive to be compressed. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | Defines tar header format. |

### setSource(File fileInfo) {#setSource-java.io.File-}
```
public final void setSource(File fileInfo)
```


Sets the content to be compressed within the archive.

Open an archive from a stream and extract it to a `MemoryStream`

```

``````

     try (Lz4Archive archive = new Lz4Archive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.lz4");
     }
 
```



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileInfo | java.io.File | Der Verweis auf eine zu komprimierende Datei. |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Legt den Inhalt fest, der im Archiv komprimiert werden soll.

```

``````

try (Lz4Archive archive = new Lz4Archive()) {
archive.setSource(new ByteArrayInputStream(new byte[] {
0x00,
(byte) 0xFF
}));
archive.save(\"archive.lz4\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | The input stream for the archive. |

### setSource(String path) {#setSource-java.lang.String-}
```
public final void setSource(String path)
```


Sets the content to be compressed within the archive.

Open an archive from file by path and extract it to a `MemoryStream`

```

``````

     try (Lz4Archive archive = new Lz4Archive()) {
         archive.setSource("data.bin");
         archive.save("archive.lz4");
     }
 
```



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | java.lang.String | Pfad zur zu komprimierenden Datei. |

