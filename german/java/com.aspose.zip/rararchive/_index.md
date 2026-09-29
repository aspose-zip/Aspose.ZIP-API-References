---
title: "RarArchive"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Diese Klasse stellt eine RAR-Archivdatei dar."
type: docs
weight: 97
url: /de/java/com.aspose.zip/rararchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class RarArchive implements IArchive, AutoCloseable
```

Diese Klasse repräsentiert eine RAR-Archivdatei. Verwenden Sie sie, um RAR-Archive zu extrahieren.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [RarArchive(String path)](#RarArchive-java.lang.String-) | Initialisiert eine neue Instanz der Klasse [RarArchive](../../com.aspose.zip/rararchive) und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann. |
| [RarArchive(String path, RarArchiveLoadOptions loadOptions)](#RarArchive-java.lang.String-com.aspose.zip.RarArchiveLoadOptions-) | Initialisiert eine neue Instanz der Klasse [RarArchive](../../com.aspose.zip/rararchive) und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann. |
| [RarArchive(InputStream sourceStream)](#RarArchive-java.io.InputStream-) | Initialisiert eine neue Instanz der Klasse [RarArchive](../../com.aspose.zip/rararchive) und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann. |
| [RarArchive(InputStream sourceStream, RarArchiveLoadOptions loadOptions)](#RarArchive-java.io.InputStream-com.aspose.zip.RarArchiveLoadOptions-) | Initialisiert eine neue Instanz der Klasse [RarArchive](../../com.aspose.zip/rararchive) und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrahiert alle Dateien im Archiv in das angegebene Verzeichnis. |
| [getEntries()](#getEntries--) | Liefert Einträge des Typs [RarArchiveEntry](../../com.aspose.zip/rararchiveentry), die das RAR-Archiv bilden. |
| [getFileEntries()](#getFileEntries--) | Liefert Einträge des Typs [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), die das RAR-Archiv bilden. |
| [getFormat()](#getFormat--) | Liefert das Archivformat. |
### RarArchive(String path) {#RarArchive-java.lang.String-}
```
public RarArchive(String path)
```


Initialisiert eine neue Instanz der Klasse [RarArchive](../../com.aspose.zip/rararchive) und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann.

Das folgende Beispiel extrahiert ein Archiv und dekomprimiert anschließend den ersten Eintrag in einen `MemoryStream`.

```

``````

ByteArrayOutputStream extracted = new ByteArrayOutputStream();
try (RarArchive archive = new RarArchive("data.rar")) {
try (InputStream decompressed = archive.getEntries().get(0).open()) {
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
extracted.write(b, 0, bytesRead);
} catch (IOException ex) {
}
}
 
```

This constructor does not decompress any entry. See [RarArchiveEntry.open()](../../com.aspose.zip/rararchiveentry\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The fully qualified or the relative path to the archive file. |

### RarArchive(String path, RarArchiveLoadOptions loadOptions) {#RarArchive-java.lang.String-com.aspose.zip.RarArchiveLoadOptions-}
```
public RarArchive(String path, RarArchiveLoadOptions loadOptions)
```


Initializes a new instance of the [RarArchive](../../com.aspose.zip/rararchive) class and composes an entry list can be extracted from the archive.

The following example extracts an archive, then decompress first entry to a `MemoryStream`.

```

``````

     ByteArrayOutputStream extracted = new ByteArrayOutputStream();
     try (RarArchive archive = new RarArchive("data.rar")) {
         try (InputStream decompressed = archive.getEntries().get(0).open()) {
             byte[] b = new byte[8192];
             int bytesRead;
             while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
                 extracted.write(b, 0, bytesRead);
         } catch (IOException ex) {
         }
     }
 
```

Dieser Konstruktor dekomprimiert keinen Eintrag. Siehe die Methode [RarArchiveEntry.open()](../../com.aspose.zip/rararchiveentry\#open--) zum Dekomprimieren.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | java.lang.String | Der vollqualifizierte oder relative Pfad zur Archivdatei. |
| loadOptions | [RarArchiveLoadOptions](../../com.aspose.zip/rararchiveloadoptions) | Optionen zum Laden eines bestehenden Archivs. |

### RarArchive(InputStream sourceStream) {#RarArchive-java.io.InputStream-}
```
public RarArchive(InputStream sourceStream)
```


Initialisiert eine neue Instanz der Klasse [RarArchive](../../com.aspose.zip/rararchive) und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann.


Das folgende Beispiel entschlüsselt und dekomprimiert den ersten Eintrag in einen `MemoryStream`.

```

``````

try (FileInputStream fs = new FileInputStream("encrypted.rar")) {
ByteArrayOutputStream extracted = new ByteArrayOutputStream();
RarArchiveLoadOptions options = new RarArchiveLoadOptions();
options.setDecryptionPassword("p@s$");
try (RarArchive archive = new RarArchive(fs, options)) {
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

This constructor does not decompress any entry. See [RarArchiveEntry.open()](../../com.aspose.zip/rararchiveentry\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | The source of the archive. |

### RarArchive(InputStream sourceStream, RarArchiveLoadOptions loadOptions) {#RarArchive-java.io.InputStream-com.aspose.zip.RarArchiveLoadOptions-}
```
public RarArchive(InputStream sourceStream, RarArchiveLoadOptions loadOptions)
```


Initializes a new instance of the [RarArchive](../../com.aspose.zip/rararchive) class and composes an entry list can be extracted from the archive.


The following example decipher and decompress first entry to a `MemoryStream`.

```

``````

     try (FileInputStream fs = new FileInputStream("encrypted.rar")) {
         ByteArrayOutputStream extracted = new ByteArrayOutputStream();
         RarArchiveLoadOptions options = new RarArchiveLoadOptions();
         options.setDecryptionPassword("p@s$");
         try (RarArchive archive = new RarArchive(fs, options)) {
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

Dieser Konstruktor dekomprimiert keinen Eintrag. Siehe die Methode [RarArchiveEntry.open()](../../com.aspose.zip/rararchiveentry\#open--) zum Dekomprimieren.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceStream | java.io.InputStream | Die Quelle des Archivs. |
| loadOptions | [RarArchiveLoadOptions](../../com.aspose.zip/rararchiveloadoptions) | Optionen zum Laden eines bestehenden Archivs. |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extrahiert alle Dateien im Archiv in das angegebene Verzeichnis.

```

``````

try (RarArchive archive = new RarArchive("archive.rar")) {
archive.extractToDirectory("C:\\extracted");
}
 
```

If the directory does not exist, it will be created.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | The path to the directory to place the extracted files in. |

### getEntries() {#getEntries--}
```
public final List<RarArchiveEntry> getEntries()
```


Gets entries of [RarArchiveEntry](../../com.aspose.zip/rararchiveentry) type constituting the rar archive.

**Returns:**
java.util.List&lt;com.aspose.zip.RarArchiveEntry&gt; - entries of [RarArchiveEntry](../../com.aspose.zip/rararchiveentry) type constituting the rar archive.
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the rar archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the rar archive.
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Gets the archive format.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
