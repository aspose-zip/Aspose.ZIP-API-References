---
title: "RarArchiveEntry"
second_title: "Aspose.ZIP för Java API-referens"
description: "Representerar en enskild fil i arkivet."
type: docs
weight: 98
url: /sv/java/com.aspose.zip/rararchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class RarArchiveEntry implements IArchiveFileEntry
```

Representerar en enskild fil i arkivet.

Kasta en [RarArchiveEntry](../../com.aspose.zip/rararchiveentry)-instans till [RarArchiveEntryEncrypted](../../com.aspose.zip/rararchiveentryencrypted) för att avgöra om posten är krypterad eller inte.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extraherar posten till den angivna strömmen. |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | Extraherar posten till den angivna strömmen. |
| [extract(String path)](#extract-java.lang.String-) | Extraherar posten till filsystemet enligt den angivna sökvägen. |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | Extraherar posten till filsystemet enligt den angivna sökvägen. |
| [getCompressedSize()](#getCompressedSize--) | Hämtar storleken på den komprimerade filen. |
| [getCreationTime()](#getCreationTime--) | Hämtar skapelsedatum och tid. |
| [getExtractionProgressed()](#getExtractionProgressed--) | Hämtar en händelse som utlöses när en del av råströmmen har extraherats. |
| [getLastAccessTime()](#getLastAccessTime--) | Hämtar senaste åtkomstdatum och tid. |
| [getLength()](#getLength--) | Hämtar längd. |
| [getModificationTime()](#getModificationTime--) | Hämtar senaste ändringsdatum och -tid. |
| [getName()](#getName--) | Hämtar namnet på posten i arkivet. |
| [getUncompressedSize()](#getUncompressedSize--) | Hämtar storleken på den ursprungliga filen. |
| [isDirectory()](#isDirectory--) | Hämtar ett värde som indikerar om posten representerar en katalog. |
| [open()](#open--) | Öppnar posten för extraktion och tillhandahåller en ström med dekomprimerat postinnehåll. |
| [open(String password)](#open-java.lang.String-) | Öppnar posten för extraktion och tillhandahåller en ström med dekomprimerat postinnehåll. |
| [setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Ställer in en händelse som utlöses när en del av råströmmen har extraherats. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extraherar posten till den angivna strömmen.


Extrahera ett objekt från rar‑arkivet med lösenord.

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| mål | java.io.OutputStream | Destinationsström. Måste vara skrivbar. |
| lösenord | java.lang.String | Valfritt lösenord för dekryptering. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extraherar posten till filsystemet enligt den angivna sökvägen.


Extrahera två poster från rar‑arkivet.

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| path | java.lang.String | Sökvägen till destinationsfilen. Om filen redan finns kommer den att skrivas över. |
| lösenord | java.lang.String | Valfritt lösenord för dekryptering. |

**Returns:**
java.io.File - filinformationen för den extraherade filen
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Hämtar storleken på den komprimerade filen.

**Returns:**
long - storleken på den komprimerade filen
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


Hämtar skapelsedatum och tid.

**Returns:**
java.util.Date - skapelsedatum och tid.
### getExtractionProgressed() {#getExtractionProgressed--}
```
public final Event<ProgressEventArgs> getExtractionProgressed()
```


Hämtar en händelse som utlöses när en del av råströmmen har extraherats.

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

Läs från strömmen för att få filens ursprungliga innehåll. Se avsnittet exempel.

**Returns:**
java.io.InputStream - Strömmen som representerar innehållet i posten.
### open(String password) {#open-java.lang.String-}
```
public final InputStream open(String password)
```


Öppnar posten för extraktion och tillhandahåller en ström med dekomprimerat postinnehåll.


Användning:

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

Event-avsändaren är en [RarArchiveEntry](../../com.aspose.zip/rararchiveentry) instans.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | en händelse som utlöses när en del av den råa strömmen har extraherats. |

