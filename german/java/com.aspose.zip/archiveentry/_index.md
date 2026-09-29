---
title: "ArchiveEntry"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Stellt eine einzelne Datei innerhalb des Archivs dar."
type: docs
weight: 27
url: /de/java/com.aspose.zip/archiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class ArchiveEntry implements IArchiveFileEntry
```

Stellt eine einzelne Datei innerhalb des Archivs dar.

Wandeln Sie eine [ArchiveEntry](../../com.aspose.zip/archiveentry)-Instanz in [ArchiveEntryEncrypted](../../com.aspose.zip/archiveentryencrypted) um, um festzustellen, ob der Eintrag verschlüsselt ist oder nicht.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrahiert den Eintrag in den bereitgestellten Stream. |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | Extrahiert den Eintrag in den bereitgestellten Stream. |
| [extract(String path)](#extract-java.lang.String-) | Extrahiert den Eintrag in das Dateisystem über den angegebenen Pfad. |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | Extrahiert den Eintrag in das Dateisystem über den angegebenen Pfad. |
| [getComment()](#getComment--) | Ermittelt den Kommentar des Eintrags im Archiv. |
| [getCompressedSize()](#getCompressedSize--) | Ermittelt die Größe der komprimierten Datei. |
| [getCompressionProgressed()](#getCompressionProgressed--) | Gibt ein Ereignis zurück, das ausgelöst wird, wenn ein Teil des Rohstreams komprimiert wird. |
| [getCompressionSettings()](#getCompressionSettings--) | Ermittelt die Einstellungen für Kompression oder Dekompression. |
| [getDataSource()](#getDataSource--) | Quelle für den Eintrag, wenn der Eintrag dem Archiv hinzugefügt wurde, nicht extrahiert. |
| [getExtractionProgressed()](#getExtractionProgressed--) | Liefert ein Ereignis, das ausgelöst wird, wenn ein Teil des Rohstreams extrahiert wird. |
| [getLength()](#getLength--) | Liefert die Länge. |
| [getModificationTime()](#getModificationTime--) | Ermittelt das Datum und die Uhrzeit der letzten Änderung. |
| [getName()](#getName--) | Liefert den Namen des Eintrags im Archiv. |
| [getUncompressedSize()](#getUncompressedSize--) | Liefert die Größe der Originaldatei. |
| [isDirectory()](#isDirectory--) | Liefert einen Wert, der angibt, ob der Eintrag ein Verzeichnis darstellt. |
| [open()](#open--) | Öffnet den Eintrag zum Extrahieren und stellt einen Stream mit dem dekomprimierten Eintragsinhalt bereit. |
| [open(String password)](#open-java.lang.String-) | Öffnet den Eintrag zum Extrahieren und stellt einen Stream mit dem dekomprimierten Eintragsinhalt bereit. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Setzt ein Ereignis, das ausgelöst wird, wenn ein Teil des Rohstreams komprimiert wird. |
| [setExtractionProgressed(Event&lt;ProgressCancelEventArgs&gt; value)](#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressCancelEventArgs--) | Setzt ein Ereignis, das ausgelöst wird, wenn ein Teil des Rohstreams extrahiert wird. |
| [setModificationTime(Date value)](#setModificationTime-java.util.Date-) | Setzt das Datum und die Uhrzeit der letzten Änderung. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extrahiert den Eintrag in den bereitgestellten Stream.

Extrahiert einen Eintrag aus einem ZIP-Archiv mit Passwort.

```

``````

try (FileInputStream zipFile = new FileInputStream("archive.zip")) {
try (Archive archive = new Archive(zipFile)) {
archive.getEntries().get(0).extract(outputStream, "p@s$");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | Destination stream. Must be writable. |

### extract(OutputStream destination, String password) {#extract-java.io.OutputStream-java.lang.String-}
```
public final void extract(OutputStream destination, String password)
```


Extracts the entry to the stream provided.

Extract an entry of zip archive with password.

```

``````

    try (FileInputStream zipFile = new FileInputStream("archive.zip")) {
        try (Archive archive = new Archive(zipFile)) {
            archive.getEntries().get(0).extract(outputStream, "p@s$");
        }
    } catch (IOException ex) {
    }
 
```



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Ziel | java.io.OutputStream | Ziel-Stream. Muss beschreibbar sein. |
| password | java.lang.String | Optionales Passwort für die Entschlüsselung. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extrahiert den Eintrag in das Dateisystem über den angegebenen Pfad.

Extrahiere zwei Einträge aus einem ZIP-Archiv, jeder mit eigenem Passwort

```

``````

try (FileInputStream zipFile = new FileInputStream("archive.zip")) {
try (Archive archive = new Archive(zipFile)) {
archive.getEntries().get(0).extract("first.bin", "first_pass");
archive.getEntries().get(1).extract("second.bin", "second_pass");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path to destination file. If the file already exists, it will be overwritten. |

**Returns:**
java.io.File - the file info of the extracted file
### extract(String path, String password) {#extract-java.lang.String-java.lang.String-}
```
public final File extract(String path, String password)
```


Extracts the entry to the filesystem by the path provided.

Extract two entries of ZIP archive, each with own password

```

``````

    try (FileInputStream zipFile = new FileInputStream("archive.zip")) {
        try (Archive archive = new Archive(zipFile)) {
            archive.getEntries().get(0).extract("first.bin", "first_pass");
            archive.getEntries().get(1).extract("second.bin", "second_pass");
        }
    } catch (IOException ex) {
    }
 
```



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | java.lang.String | Der Pfad zur Zieldatei. Wenn die Datei bereits existiert, wird sie überschrieben. |
| password | java.lang.String | Optionales Passwort für die Entschlüsselung. |

**Returns:**
java.io.File - die Dateiinformation der extrahierten Datei
### getComment() {#getComment--}
```
public final String getComment()
```


Ermittelt den Kommentar des Eintrags im Archiv.

**Returns:**
java.lang.String - Kommentar des Eintrags im Archiv
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Ermittelt die Größe der komprimierten Datei.

**Returns:**
long - Größe der komprimierten Datei
### getCompressionProgressed() {#getCompressionProgressed--}
```
public final Event<ProgressEventArgs> getCompressionProgressed()
```


Gibt ein Ereignis zurück, das ausgelöst wird, wenn ein Teil des Rohstreams komprimiert wird.

```

``````

archive.getEntries().get(0).setCompressionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
}
});
 
```

Event sender is an [ArchiveEntry](../../com.aspose.zip/archiveentry) instance.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream compressed
### getCompressionSettings() {#getCompressionSettings--}
```
public final CompressionSettings getCompressionSettings()
```


Gets settings for compression or decompression.

**Returns:**
[CompressionSettings](../../com.aspose.zip/compressionsettings) - settings for compression or decompression.
### getDataSource() {#getDataSource--}
```
public final InputStream getDataSource()
```


Source for the entry if the entry was added to the archive, not extracted.

Before assigned, the source is null. This source may be assigned within `Archive.save` method in some cases.

**Returns:**
java.io.InputStream - the source for the entry
### getExtractionProgressed() {#getExtractionProgressed--}
```
public final Event<ProgressCancelEventArgs> getExtractionProgressed()
```


Gets an event that is raised when a portion of raw stream extracted.

In this sample event handler is used for calculation the share of proceeded size in percents.

```

``````

    archive.getEntries().get(0).setExtractionProgressed(new Event<ProgressEventArgs>() {
        public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
            int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / ((ArchiveEntry) sender).getUncompressedSize());
        }
    });
 
```

In diesem Beispiel wird der Ereignishandler zum Abbruch verwendet, nachdem die ersten hundert MB des Eintrags extrahiert wurden.

```

``````

a.getEntries().get(0).setExtractionProgressed( (s, e) -> { if (e.getProceededBytes() > 100000000) e.setCancel(true); } );
 
```

Event sender is an [ArchiveEntry](../../com.aspose.zip/archiveentry) instance. It is possible to cancel extraction.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream extracted.
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets length.

**Returns:**
java.lang.Long - length
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Gets last modified date and time.

**Returns:**
java.util.Date - last modified date and time
### getName() {#getName--}
```
public final String getName()
```


Gets name of the entry within the archive.

**Returns:**
java.lang.String - name of the entry within the archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets size of the original file.

**Returns:**
long - size of the original file
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Gets a value indicating whether the entry represents a directory.

**Returns:**
boolean - a value indicating whether the entry represents a directory.
### open() {#open--}
```
public final InputStream open()
```


Opens the entry for extraction and provides a stream with decompressed entry content.


Usage:

```

``````

    InputStream decompressed = entry.open();
    byte[] buffer = new byte[8192];
    int bytesRead;
    while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length)))
        fileStream.write(buffer, 0, bytesRead);
 
```

Lesen Sie aus dem Stream, um den ursprünglichen Inhalt der Datei zu erhalten.

**Returns:**
java.io.InputStream - Der Stream, der den Inhalt des Eintrags darstellt.
### open(String password) {#open-java.lang.String-}
```
public final InputStream open(String password)
```


Öffnet den Eintrag zum Extrahieren und stellt einen Stream mit dem dekomprimierten Eintragsinhalt bereit.


Verwendung:

```

``````

InputStream decompressed = entry.open();
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length)))
fileStream.write(buffer, 0, bytesRead);
 
```

Read from the stream to get the original content of the file. See examples section.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | java.lang.String | Optional password for decryption. |

**Returns:**
java.io.InputStream - The stream that represents the contents of the entry.
### setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public final void setCompressionProgressed(Event<ProgressEventArgs> value)
```


Sets an event that is raised when a portion of raw stream compressed.

```

``````

    archive.getEntries().get(0).setCompressionProgressed(new Event<ProgressEventArgs>() {
        public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
            int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
        }
    });
 
```

Der Ereignisabsender ist eine [ArchiveEntry](../../com.aspose.zip/archiveentry) Instanz.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | ein Ereignis, das ausgelöst wird, wenn ein Teil des Rohstreams komprimiert wird |

### setExtractionProgressed(Event&lt;ProgressCancelEventArgs&gt; value) {#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressCancelEventArgs--}
```
public final void setExtractionProgressed(Event<ProgressCancelEventArgs> value)
```


Setzt ein Ereignis, das ausgelöst wird, wenn ein Teil des Rohstreams extrahiert wird.

In diesem Beispiel wird der Ereignishandler zur Berechnung des Anteils der verarbeiteten Größe in Prozent verwendet.

```

``````

archive.getEntries().get(0).setExtractionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / ((ArchiveEntry) sender).getUncompressedSize());
}
});
 
```

In this sample event handler is used for cancellation after the first hundred of Mb of entry was extracted.

```

``````

 a.getEntries().get(0).setExtractionProgressed( (s, e) -> { if (e.getProceededBytes() > 100000000) e.setCancel(true); } );
 
```

Der Ereignisabsender ist eine [ArchiveEntry](../../com.aspose.zip/archiveentry) Instanz. Es ist möglich, die Extraktion abzubrechen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | com.aspose.zip.Event&lt;com.aspose.zip.ProgressCancelEventArgs&gt; | ein Ereignis, das ausgelöst wird, wenn ein Teil des Rohstreams extrahiert wurde. |

### setModificationTime(Date value) {#setModificationTime-java.util.Date-}
```
public final void setModificationTime(Date value)
```


Setzt das Datum und die Uhrzeit der letzten Änderung.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Date | letztes Änderungsdatum und -uhrzeit |

