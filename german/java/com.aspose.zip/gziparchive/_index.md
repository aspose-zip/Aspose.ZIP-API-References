---
title: "GzipArchive"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Diese Klasse stellt eine gzip-Archivdatei dar."
type: docs
weight: 69
url: /de/java/com.aspose.zip/gziparchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class GzipArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

Diese Klasse repräsentiert eine gzip-Archivdatei. Verwenden Sie sie, um gzip-Archive zu erstellen oder zu extrahieren.

Der Gzip-Komprimierungsalgorithmus basiert auf dem DEFLATE-Algorithmus, der eine Kombination aus LZ77 und Huffman-Codierung ist.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [GzipArchive()](#GzipArchive--) | Initialisiert eine neue Instanz der [GzipArchive](../../com.aspose.zip/gziparchive) Klasse, die zum Komprimieren vorbereitet ist. |
| [GzipArchive(InputStream sourceStream)](#GzipArchive-java.io.InputStream-) | Initialisiert eine neue Instanz der [GzipArchive](../../com.aspose.zip/gziparchive) Klasse, die zum Dekomprimieren vorbereitet ist. |
| [GzipArchive(InputStream sourceStream, boolean parseHeader)](#GzipArchive-java.io.InputStream-boolean-) | Initialisiert eine neue Instanz der [GzipArchive](../../com.aspose.zip/gziparchive) Klasse, die zum Dekomprimieren vorbereitet ist. |
| [GzipArchive(InputStream sourceStream, GzipLoadOptions options)](#GzipArchive-java.io.InputStream-com.aspose.zip.GzipLoadOptions-) | Initialisiert eine neue Instanz der [GzipArchive](../../com.aspose.zip/gziparchive) Klasse, die zum Dekomprimieren vorbereitet ist. |
| [GzipArchive(String path, GzipLoadOptions options)](#GzipArchive-java.lang.String-com.aspose.zip.GzipLoadOptions-) | Initialisiert eine neue Instanz der [GzipArchive](../../com.aspose.zip/gziparchive) Klasse, die zum Dekomprimieren vorbereitet ist. |
| [GzipArchive(String path)](#GzipArchive-java.lang.String-) | Initialisiert eine neue Instanz der [GzipArchive](../../com.aspose.zip/gziparchive) Klasse. |
| [GzipArchive(String path, boolean parseHeader)](#GzipArchive-java.lang.String-boolean-) | Initialisiert eine neue Instanz der [GzipArchive](../../com.aspose.zip/gziparchive) Klasse. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrahiert das Archiv in den bereitgestellten Stream. |
| [extract(String path)](#extract-java.lang.String-) | Extrahiert das Archiv in die Datei anhand des Pfads. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrahiert den Inhalt des Archivs in das angegebene Verzeichnis. |
| [getFileEntries()](#getFileEntries--) | Ruft Einträge des Typs [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) ab, die das gzip-Archiv bilden. |
| [getFormat()](#getFormat--) | Liefert das Archivformat. |
| [getLength()](#getLength--) | Ruft die Größe einer Originaldatei ab. |
| [getName()](#getName--) | Der Name der Originaldatei. |
| [getUncompressedSize()](#getUncompressedSize--) | Ruft die Größe einer Originaldatei ab. |
| [open()](#open--) | Öffnet das Archiv zum Extrahieren und stellt einen Stream mit dem Archivinhalt bereit. |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | Speichert das Archiv in den angegebenen Stream. |
| [save(String destinationFileName)](#save-java.lang.String-) | Speichert das Archiv in die angegebene Zieldatei. |
| [setSource(TarArchive tarArchive)](#setSource-com.aspose.zip.TarArchive-) | Legt den Inhalt fest, der im Archiv komprimiert werden soll. |
| [setSource(File file)](#setSource-java.io.File-) | Legt den Inhalt fest, der im Archiv komprimiert werden soll. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Legt den Inhalt fest, der im Archiv komprimiert werden soll. |
| [setSource(String path)](#setSource-java.lang.String-) | Legt den Inhalt fest, der im Archiv komprimiert werden soll. |
### GzipArchive() {#GzipArchive--}
```
public GzipArchive()
```


Initialisiert eine neue Instanz der [GzipArchive](../../com.aspose.zip/gziparchive) Klasse, die zum Komprimieren vorbereitet ist.

Das folgende Beispiel zeigt, wie man eine Datei komprimiert.

```

``````

try (GzipArchive archive = new GzipArchive())
{
archive.setSource("data.bin");
archive.save("archive.gz");
}
 
```



### GzipArchive(InputStream sourceStream) {#GzipArchive-java.io.InputStream-}
```
public GzipArchive(InputStream sourceStream)
```


Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class prepared for decompressing.

Open an archive from a stream and extract it to a `ByteArrayOutputStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (GzipArchive archive = new GzipArchive(Files.newInputStream(java.nio.file.Paths.get("archive.gz")))) {
         byte[] b = new byte[8192];
         int bytesRead;
         InputStream archiveStream = archive.open();
         while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

Dieser Konstruktor dekomprimiert nicht. Siehe die Methode [open()](../../com.aspose.zip/gziparchive\\#open--) zum Dekomprimieren.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceStream | java.io.InputStream | Die Quelle des Archivs. |

### GzipArchive(InputStream sourceStream, boolean parseHeader) {#GzipArchive-java.io.InputStream-boolean-}
```
public GzipArchive(InputStream sourceStream, boolean parseHeader)
```


Initialisiert eine neue Instanz der [GzipArchive](../../com.aspose.zip/gziparchive) Klasse, die zum Dekomprimieren vorbereitet ist.

Öffnen Sie ein Archiv aus einem Stream und extrahieren Sie es in einen `ByteArrayOutputStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (GzipArchive archive = new GzipArchive(Files.newInputStream(java.nio.file.Paths.get("archive.gz")))) {
byte[] b = new byte[8192];
int bytesRead;
InputStream archiveStream = archive.open();
while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/gziparchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | The source of the archive. |
| parseHeader | boolean | Whether to parse stream header to figure out properties, including name. Makes sense for seekable stream only. |

### GzipArchive(InputStream sourceStream, GzipLoadOptions options) {#GzipArchive-java.io.InputStream-com.aspose.zip.GzipLoadOptions-}
```
public GzipArchive(InputStream sourceStream, GzipLoadOptions options)
```


Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class prepared for decompressing.

Open an archive from a stream and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     GzipLoadOptions options = new GzipLoadOptions();
     try (GzipArchive archive = new GzipArchive(new FileInputStream("archive.gz"), options)) {
         archive.extract(ms);
     } catch (IOException ex) {
     }
 
```

Dieser Konstruktor dekomprimiert nicht. Siehe die Methode [open()](../../com.aspose.zip/gziparchive\\#open--) zum Dekomprimieren.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceStream | java.io.InputStream | Die Quelle des Archivs. |
| options | [GzipLoadOptions](../../com.aspose.zip/gziploadoptions) | Optionen zum Laden des Archivs. |

### GzipArchive(String path, GzipLoadOptions options) {#GzipArchive-java.lang.String-com.aspose.zip.GzipLoadOptions-}
```
public GzipArchive(String path, GzipLoadOptions options)
```


Initialisiert eine neue Instanz der [GzipArchive](../../com.aspose.zip/gziparchive) Klasse, die zum Dekomprimieren vorbereitet ist.

Öffnen Sie ein Archiv aus einer Datei über den Pfad und extrahieren Sie es in einen `MemoryStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
GzipLoadOptions options = new GzipLoadOptions();
try (GzipArchive archive = new GzipArchive("archive.gz", options)) {
archive.extract(ms);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/gziparchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path to the archive file. |
| options | [GzipLoadOptions](../../com.aspose.zip/gziploadoptions) | Options to load the archive with. |

### GzipArchive(String path) {#GzipArchive-java.lang.String-}
```
public GzipArchive(String path)
```


Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class.

Open an archive from file by path and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (GzipArchive archive = new GzipArchive("archive.gz")) {
         byte[] b = new byte[8192];
         int bytesRead;
         InputStream archiveStream = archive.open();
         while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

Dieser Konstruktor dekomprimiert nicht. Siehe die Methode [open()](../../com.aspose.zip/gziparchive\\#open--) zum Dekomprimieren.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | java.lang.String | Der Pfad zur Archivdatei. |

### GzipArchive(String path, boolean parseHeader) {#GzipArchive-java.lang.String-boolean-}
```
public GzipArchive(String path, boolean parseHeader)
```


Initialisiert eine neue Instanz der [GzipArchive](../../com.aspose.zip/gziparchive) Klasse.

Öffnen Sie ein Archiv aus einer Datei über den Pfad und extrahieren Sie es in einen `MemoryStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (GzipArchive archive = new GzipArchive("archive.gz")) {
byte[] b = new byte[8192];
int bytesRead;
InputStream archiveStream = archive.open();
while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/gziparchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path to the archive file. |
| parseHeader | boolean | Whether to parse stream header to figure out properties, including name. Makes sense for seekable stream only. |

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

     try (GzipArchive archive = new GzipArchive("archive.gz")) {
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


Ruft Einträge des Typs [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) ab, die das gzip-Archiv bilden.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - Einträge des Typs [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), die das gzip-Archiv bilden.
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


Ruft die Größe einer Originaldatei ab.

Während der Dekompression kann diese Eigenschaft eine falsche Größe enthalten. Wenn die Größe der dekomprimierten Datei 4 GB überschreitet, liefert diese Eigenschaft aufgrund der 32‑Bit‑Begrenzung im Header einen falschen Wert.

**Returns:**
java.lang.Long - Größe einer Originaldatei
### getName() {#getName--}
```
public final String getName()
```


Der Name der Originaldatei.

**Returns:**
java.lang.String - der Name der Originaldatei
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Ruft die Größe einer Originaldatei ab.

Während der Dekompression kann diese Eigenschaft eine falsche Größe enthalten. Wenn die Größe der dekomprimierten Datei 4 GB überschreitet, liefert diese Eigenschaft aufgrund der 32‑Bit‑Begrenzung im Header einen falschen Wert.

**Returns:**
long - Größe einer Originaldatei.
### open() {#open--}
```
public final InputStream open()
```


Öffnet das Archiv zum Extrahieren und stellt einen Stream mit dem Archivinhalt bereit.

Extrahiert das Archiv und kopiert den extrahierten Inhalt in den Dateistream.

```

``````

try (GzipArchive archive = new GzipArchive("archive.gz")) {
try (FileOutputStream extracted = new FileOutputStream("data.bin")) {
InputStream unpacked = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = unpacked.read(b, 0, b.length))) {
extracted.write(b, 0, bytesRead);
}
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

Read from the stream to get the original content of a file. See examples section.

**Returns:**
java.io.InputStream - The stream that represents the contents of the archive.
### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


Saves archive to the stream provided.

Writes compressed data to http response stream.

```

``````

     try (GzipArchive archive = new GzipArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(httpResponseStream);
     }
 
```



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | outputStream | java.io.OutputStream | Ziel-Stream. |

`outputStream` muss beschreibbar sein. |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Speichert das Archiv in die angegebene Zieldatei.

```

``````

try (GzipArchive archive = new GzipArchive()) {
archive.setSource("data.bin");
archive.save("archive.gz");
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
         try (GzipArchive gzippedArchive = new GzipArchive()) {
             gzippedArchive.setSource(tarArchive);
             gzippedArchive.save("archive.tar.gz");
         }
     }
 
```

Verwenden Sie diese Methode, um ein gemeinsames tar.gz-Archiv zu erstellen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| tarArchive | [TarArchive](../../com.aspose.zip/tararchive) | Tar-Archiv, das komprimiert werden soll. |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Legt den Inhalt fest, der im Archiv komprimiert werden soll.

```

``````

try (GzipArchive archive = new GzipArchive()) {
archive.setSource(new File("data.bin"));
archive.save("archive.gz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | The reference to a file to be compressed. |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Sets the content to be compressed within the archive.

```

``````

     try (GzipArchive archive = new GzipArchive()) {
         archive.setSource(new ByteArrayInputStream(new byte[] {
                 0x00,
                 (byte) 0xFF
         }));
         archive.save("archive.gz");
     }
 
```



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| source | java.io.InputStream | Der Eingabestream für das Archiv. |

### setSource(String path) {#setSource-java.lang.String-}
```
public final void setSource(String path)
```


Legt den Inhalt fest, der im Archiv komprimiert werden soll.

Öffnen Sie ein Archiv aus einer Datei über den Pfad und extrahieren Sie es in einen `MemoryStream`

```

``````

try (GzipArchive archive = new GzipArchive()) {
archive.setSource("data.bin");
archive.save("archive.gz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | Path to file to be compressed. |

