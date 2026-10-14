---
title: "UueArchive"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Diese Klasse repräsentiert eine uuencodierte Datei."
type: docs
weight: 128
url: /de/java/com.aspose.zip/uuearchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class UueArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

Diese Klasse repräsentiert eine uuencodierte Datei.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [UueArchive()](#UueArchive--) | Initialisiert eine neue Instanz der Klasse [UueArchive](../../com.aspose.zip/uuearchive), die für das Codieren vorbereitet ist. |
| [UueArchive(InputStream sourceStream)](#UueArchive-java.io.InputStream-) | Initialisiert eine neue Instanz der Klasse [UueArchive](../../com.aspose.zip/uuearchive), die für das Dekodieren vorbereitet ist. |
| [UueArchive(String path)](#UueArchive-java.lang.String-) | Initialisiert eine neue Instanz der Klasse [UueArchive](../../com.aspose.zip/uuearchive). |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrahiert das Archiv in den bereitgestellten Stream. |
| [extract(String path)](#extract-java.lang.String-) | Extrahiert das Archiv in die Datei anhand des Pfads. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrahiert den Inhalt des Archivs in das angegebene Verzeichnis. |
| [getFileEntries()](#getFileEntries--) | Ruft Einträge des Typs [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) ab, die das uue-Archiv bilden. |
| [getFormat()](#getFormat--) | Liefert das Archivformat. |
| [getLength()](#getLength--) | Liefert die Länge. |
| [getName()](#getName--) | Name der Originaldatei. |
| [open()](#open--) | Öffnet das Archiv zum Dekodieren und stellt einen Stream mit dem Archivinhalt bereit. |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | Speichert das Archiv in den angegebenen Stream. |
| [save(OutputStream outputStream, UueSaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.UueSaveOptions-) | Speichert das Archiv in den angegebenen Stream. |
| [save(String destinationFileName)](#save-java.lang.String-) | Speichert das Archiv in die angegebene Zieldatei. |
| [save(String destinationFileName, UueSaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.UueSaveOptions-) | Speichert das Archiv in die angegebene Zieldatei. |
| [setSource(File file)](#setSource-java.io.File-) | Legt den Inhalt fest, der im Archiv komprimiert werden soll. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Legt den Inhalt fest, der im Archiv codiert werden soll. |
| [setSource(String path)](#setSource-java.lang.String-) | Legt den Inhalt fest, der im Archiv codiert werden soll. |
### UueArchive() {#UueArchive--}
```
public UueArchive()
```


Initialisiert eine neue Instanz der Klasse [UueArchive](../../com.aspose.zip/uuearchive), die für das Codieren vorbereitet ist.

Das folgende Beispiel zeigt, wie man eine Datei uuencodiert.

```

``````

try (UueArchive archive = new UueArchive()) {
archive.setSource("data.bin");
archive.save("archive.uue");
}
 
```



### UueArchive(InputStream sourceStream) {#UueArchive-java.io.InputStream-}
```
public UueArchive(InputStream sourceStream)
```


Initializes a new instance of the [UueArchive](../../com.aspose.zip/uuearchive) class prepared for decoding.

Open an archive from a stream and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (UueArchive archive = new UueArchive(new FileInputStream("archive.001"))) {
         InputStream decompressed = archive.open();
         byte[] b = new byte[8192];
         int bytesRead;
         while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
     }
 
```

Dieser Konstruktor dekodiert nicht. Siehe die Methode [open()](../../com.aspose.zip/uuearchive\#open--) zum Dekomprimieren.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceStream | java.io.InputStream | die Quelle des Archivs |

### UueArchive(String path) {#UueArchive-java.lang.String-}
```
public UueArchive(String path)
```


Initialisiert eine neue Instanz der Klasse [UueArchive](../../com.aspose.zip/uuearchive).

Öffne ein Archiv aus einer Datei über den Pfad und dekodiere es in einen `MemoryStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (UueArchive archive = new UueArchive(new FileInputStream("archive.uue"))) {
InputStream decompressed = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
}
 
```

This constructor does not decode. See [open()](../../com.aspose.zip/uuearchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

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

     try (UueArchive archive = new UueArchive("archive.uue")) {
         archive.extract(httpResponseStream);
     }
 
```



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Ziel | java.io.OutputStream | Ziel-Stream |

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
java.io.File - Informationen der extrahierten Datei
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


Ruft Einträge des Typs [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) ab, die das uue-Archiv bilden.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - Einträge des Typs [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), die das uue-Archiv bilden
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


Name der Originaldatei.

**Returns:**
java.lang.String - der Name der Originaldatei
### open() {#open--}
```
public final InputStream open()
```


Öffnet das Archiv zum Dekodieren und stellt einen Stream mit dem Archivinhalt bereit.

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

Write compressed data to http response stream.

```

``````

     try (UueArchive archive = new UueArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(outputStream);
     }
 
```



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| outputStream | java.io.OutputStream | Ziel-Stream |

### save(OutputStream outputStream, UueSaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.UueSaveOptions-}
```
public final void save(OutputStream outputStream, UueSaveOptions saveOptions)
```


Speichert das Archiv in den angegebenen Stream.

Schreiben Sie komprimierte Daten in den HTTP-Antwort-Stream.

```

``````

try (UueArchive archive = new UueArchive()) {
archive.setSource(new File("data.bin"));
archive.save(outputStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outputStream | java.io.OutputStream | destination stream |
| saveOptions | [UueSaveOptions](../../com.aspose.zip/uuesaveoptions) | options for the archive saving |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves the archive to the destination file provided.

Write encoded data to file.

```

``````

     try (UueArchive archive = new UueArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("data.uue");
     }
 
```



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| destinationFileName | java.lang.String | der Pfad des zu erstellenden Archivs. Wenn der angegebene Dateiname auf eine bereits vorhandene Datei verweist, wird sie überschrieben |

### save(String destinationFileName, UueSaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.UueSaveOptions-}
```
public final void save(String destinationFileName, UueSaveOptions saveOptions)
```


Speichert das Archiv in die angegebene Zieldatei.

Kodierte Daten in Datei schreiben.

```

``````

try (UueArchive archive = new UueArchive()) {
archive.setSource(new File("data.bin"));
archive.save("data.uue");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| saveOptions | [UueSaveOptions](../../com.aspose.zip/uuesaveoptions) | options for the archive saving |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Sets the content to be compressed within the archive.

```

``````

     try (UueArchive archive = new UueArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.uue");
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


Legt den Inhalt fest, der im Archiv codiert werden soll.

```

``````

try (UueArchive archive = new UueArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] {
0x00,
(byte) 0xFF
}));
archive.save("archive.uue");
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


Sets the content to be encoded within the archive.

```

``````

     try (UueArchive archive = new UueArchive()) {
         archive.setSource("data.bin");
         archive.save("archive.uue");
     }
 
```



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | java.lang.String | Pfad zur zu kodierenden Datei |

