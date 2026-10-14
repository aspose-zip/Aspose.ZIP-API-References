---
title: "SevenZipArchiveEntry"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Stellt eine einzelne Datei innerhalb eines 7z-Archivs dar."
type: docs
weight: 105
url: /de/java/com.aspose.zip/sevenziparchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class SevenZipArchiveEntry implements IArchiveFileEntry
```

Stellt eine einzelne Datei innerhalb eines 7z-Archivs dar.

Wandeln Sie eine Instanz von [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) in [SevenZipArchiveEntryEncrypted](../../com.aspose.zip/sevenziparchiveentryencrypted) um, um zu bestimmen, ob der Eintrag verschlüsselt ist oder nicht.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrahiert den Eintrag in den bereitgestellten Stream. |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | Extrahiert den Eintrag in den bereitgestellten Stream. |
| [extract(String path)](#extract-java.lang.String-) | Extrahiert den Eintrag in das Dateisystem über den angegebenen Pfad. |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | Extrahiert den Eintrag in das Dateisystem über den angegebenen Pfad. |
| [getCompressedSize()](#getCompressedSize--) | Liefert die Größe der komprimierten Datei. |
| [getCompressionProgressed()](#getCompressionProgressed--) | Gibt ein Ereignis zurück, das ausgelöst wird, wenn ein Teil des Rohstreams komprimiert wird. |
| [getCompressionSettings()](#getCompressionSettings--) | Ermittelt die Einstellungen für Kompression oder Dekompression. |
| [getLength()](#getLength--) | Liefert die Länge. |
| [getModificationTime()](#getModificationTime--) | Ermittelt das Datum und die Uhrzeit der letzten Änderung. |
| [getName()](#getName--) | Gibt den Namen des Eintrags im Archiv zurück. |
| [getUncompressedSize()](#getUncompressedSize--) | Ermittelt die Größe der Originaldatei. |
| [isDirectory()](#isDirectory--) | Liefert einen Wert, der angibt, ob der Eintrag ein Verzeichnis darstellt. |
| [open()](#open--) | Öffnet den Eintrag zum Extrahieren und stellt einen Stream mit dem Eintragsinhalt bereit. |
| [open(String password)](#open-java.lang.String-) | Öffnet den Eintrag zum Extrahieren und stellt einen Stream mit dem Eintragsinhalt bereit. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Setzt ein Ereignis, das ausgelöst wird, wenn ein Teil des Rohstreams komprimiert wird. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extrahiert den Eintrag in den bereitgestellten Stream.

Extrahiert einen Eintrag aus einem ZIP-Archiv mit Passwort.

```

``````

try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
archive.getEntries().get(0).extract(httpResponseStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream. Must be writable |

### extract(OutputStream destination, String password) {#extract-java.io.OutputStream-java.lang.String-}
```
public final void extract(OutputStream destination, String password)
```


Extracts the entry to the stream provided.

Extract an entry of zip archive with password.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
         archive.getEntries().get(0).extract(httpResponseStream);
     }
 
```



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Ziel | java.io.OutputStream | Ziel-Stream. Muss beschreibbar sein. |
| password | java.lang.String | Optionales Passwort für die Entschlüsselung |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extrahiert den Eintrag in das Dateisystem über den angegebenen Pfad.

```

``````

try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
archive.getEntries().get(0).extract(\"data.bin\");
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

```

``````

     try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
         archive.getEntries().get(0).extract("data.bin");
     }
 
```



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | java.lang.String | Der Pfad zur Zieldatei. Wenn die Datei bereits existiert, wird sie überschrieben. |
| password | java.lang.String | Optionales Passwort für die Entschlüsselung |

**Returns:**
java.io.File - die Dateiinformation der extrahierten Datei
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Liefert die Größe der komprimierten Datei.

**Returns:**
long – die Größe der komprimierten Datei
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

Event sender is an [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) instance.

Does not invoke in solid mode and in multithreaded mode for LZMA2 entries.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream compressed
### getCompressionSettings() {#getCompressionSettings--}
```
public final SevenZipCompressionSettings getCompressionSettings()
```


Gets settings for compression or decompression.

**Returns:**
[SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) - settings for compression or decompression
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


Gets the name of the entry within the archive.

**Returns:**
java.lang.String - the name of the entry within the archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets the size of the original file.

**Returns:**
long - the size of the original file
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Gets a value indicating whether the entry represents a directory.

**Returns:**
boolean - a value indicating whether the entry represents a directory
### open() {#open--}
```
public final InputStream open()
```


Opens the entry for extraction and provides a stream with entry content.

Usage:

```

``````

     SevenZipArchive archive = new SevenZipArchive("archive.7z");
     SevenZipArchiveEntry entry = archive.getEntries().get(0);
     try (FileOutputStream fileStream = new FileOutputStream("data.bin")) {
         try (InputStream decompressed = entry.open()) {
             byte[] buffer = new byte[8192];
             int bytesRead;
             while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
                 fileStream.write(buffer, 0, bytesRead);
             }
         }
     } catch (IOException ex) {
     }
 
```

Lesen Sie aus dem Stream, um den ursprünglichen Inhalt der Datei zu erhalten. Siehe den Abschnitt Beispiele.

**Returns:**
java.io.InputStream - der Stream, der den Inhalt des Eintrags darstellt.
### open(String password) {#open-java.lang.String-}
```
public final InputStream open(String password)
```


Öffnet den Eintrag zum Extrahieren und stellt einen Stream mit dem Eintragsinhalt bereit.

Verwendung:

```

``````

SevenZipArchive archive = new SevenZipArchive(\"archive.7z\");
SevenZipArchiveEntry entry = archive.getEntries().get(0);
try (FileOutputStream fileStream = new FileOutputStream("data.bin")) {
try (InputStream decompressed = entry.open()) {
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
fileStream.write(buffer, 0, bytesRead);
}
}
} catch (IOException ex) {
}
 
```

Read from the stream to get the original content of the file. See examples section.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | java.lang.String | optional password for decryption |

**Returns:**
java.io.InputStream - the stream that represents the contents of the entry
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

Der Ereignisabsender ist eine [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) Instanz.

Wird im Solid‑Modus und im Mehrthread‑Modus für LZMA2‑Einträge nicht aufgerufen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | ein Ereignis, das ausgelöst wird, wenn ein Teil des Rohstreams komprimiert wird |

