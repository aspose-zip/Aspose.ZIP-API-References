---
title: "RarArchiveEntry"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Stellt eine einzelne Datei innerhalb des Archivs dar."
type: docs
weight: 98
url: /de/java/com.aspose.zip/rararchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class RarArchiveEntry implements IArchiveFileEntry
```

Stellt eine einzelne Datei innerhalb des Archivs dar.

Wandeln Sie eine [RarArchiveEntry](../../com.aspose.zip/rararchiveentry)-Instanz in [RarArchiveEntryEncrypted](../../com.aspose.zip/rararchiveentryencrypted) um, um zu bestimmen, ob der Eintrag verschlüsselt ist oder nicht.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrahiert den Eintrag in den bereitgestellten Stream. |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | Extrahiert den Eintrag in den bereitgestellten Stream. |
| [extract(String path)](#extract-java.lang.String-) | Extrahiert den Eintrag in das Dateisystem über den angegebenen Pfad. |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | Extrahiert den Eintrag in das Dateisystem über den angegebenen Pfad. |
| [getCompressedSize()](#getCompressedSize--) | Ermittelt die Größe der komprimierten Datei. |
| [getCreationTime()](#getCreationTime--) | Ermittelt Erstellungsdatum und -zeit. |
| [getExtractionProgressed()](#getExtractionProgressed--) | Liefert ein Ereignis, das ausgelöst wird, wenn ein Teil des Rohstreams extrahiert wird. |
| [getLastAccessTime()](#getLastAccessTime--) | Ermittelt das Datum und die Uhrzeit des letzten Zugriffs. |
| [getLength()](#getLength--) | Liefert die Länge. |
| [getModificationTime()](#getModificationTime--) | Ermittelt das Datum und die Uhrzeit der letzten Änderung. |
| [getName()](#getName--) | Gibt den Namen des Eintrags im Archiv zurück. |
| [getUncompressedSize()](#getUncompressedSize--) | Ermittelt die Größe der Originaldatei. |
| [isDirectory()](#isDirectory--) | Liefert einen Wert, der angibt, ob der Eintrag ein Verzeichnis darstellt. |
| [open()](#open--) | Öffnet den Eintrag zum Extrahieren und stellt einen Stream mit dem dekomprimierten Eintragsinhalt bereit. |
| [open(String password)](#open-java.lang.String-) | Öffnet den Eintrag zum Extrahieren und stellt einen Stream mit dem dekomprimierten Eintragsinhalt bereit. |
| [setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Setzt ein Ereignis, das ausgelöst wird, wenn ein Teil des Rohstreams extrahiert wird. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extrahiert den Eintrag in den bereitgestellten Stream.


Extrahiert einen Eintrag aus einem RAR-Archiv mit Passwort.

```

``````

try (FileInputStream rarFile = new FileInputStream("archive.rar")) {
try (RarArchive archive = new RarArchive(rarFile)) {
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


Extract an entry of rar archive with password.

```

``````

    try (FileInputStream rarFile = new FileInputStream("archive.rar")) {
        try (RarArchive archive = new RarArchive(rarFile)) {
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


Extrahiert zwei Einträge aus einem RAR-Archiv.

```

``````

try (FileInputStream rarFile = new FileInputStream("archive.rar")) {
try (RarArchive archive = new RarArchive(rarFile)) {
archive.getEntries().get(0).extract("first.bin", "pass");
archive.getEntries().get(1).extract("second.bin", "pass");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to destination file. If the file already exists, it will be overwritten |

**Returns:**
java.io.File - the file info of the extracted file
### extract(String path, String password) {#extract-java.lang.String-java.lang.String-}
```
public final File extract(String path, String password)
```


Extracts the entry to the filesystem by the path provided.


Extract two entries of rar archive.

```

``````

    try (FileInputStream rarFile = new FileInputStream("archive.rar")) {
        try (RarArchive archive = new RarArchive(rarFile)) {
            archive.getEntries().get(0).extract("first.bin", "pass");
            archive.getEntries().get(1).extract("second.bin", "pass");
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
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Ermittelt die Größe der komprimierten Datei.

**Returns:**
long – die Größe der komprimierten Datei
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


Ermittelt Erstellungsdatum und -zeit.

**Returns:**
java.util.Date – Erstellungsdatum und -zeit.
### getExtractionProgressed() {#getExtractionProgressed--}
```
public final Event<ProgressEventArgs> getExtractionProgressed()
```


Liefert ein Ereignis, das ausgelöst wird, wenn ein Teil des Rohstreams extrahiert wird.

```

``````

archive.getEntries().get(0).setExtractionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / ((RarArchiveEntry) sender).getUncompressedSize());
}
});
 
```

Event sender is an [RarArchiveEntry](../../com.aspose.zip/rararchiveentry) instance.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream extracted.
### getLastAccessTime() {#getLastAccessTime--}
```
public final Date getLastAccessTime()
```


Gets last access date and time.

**Returns:**
java.util.Date - last access date and time.
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets length.

**Returns:**
java.lang.Long - length.
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Gets last modified date and time.

**Returns:**
java.util.Date - last modified date and time.
### getName() {#getName--}
```
public final String getName()
```


Gets the name of the entry within the archive.

**Returns:**
java.lang.String - the name of the entry within the archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets the size of the original file.

**Returns:**
long - the size of the original file.
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

Lesen Sie aus dem Stream, um den ursprünglichen Inhalt der Datei zu erhalten. Siehe den Abschnitt Beispiele.

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
| password | java.lang.String | Optional password for decryption. It can also be set within [RarArchiveLoadOptions.setDecryptionPassword(String)](../../com.aspose.zip/rararchiveloadoptions\#setDecryptionPassword-String-). |

**Returns:**
java.io.InputStream - The stream that represents the contents of the entry.
### setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public final void setExtractionProgressed(Event<ProgressEventArgs> value)
```


Sets an event that is raised when a portion of raw stream extracted.

```

``````

    archive.getEntries().get(0).setExtractionProgressed(new Event<ProgressEventArgs>() {
        public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
            int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / ((RarArchiveEntry) sender).getUncompressedSize());
        }
    });
 
```

Event-Absender ist eine Instanz von [RarArchiveEntry](../../com.aspose.zip/rararchiveentry).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | ein Ereignis, das ausgelöst wird, wenn ein Teil des Rohstreams extrahiert wurde. |

