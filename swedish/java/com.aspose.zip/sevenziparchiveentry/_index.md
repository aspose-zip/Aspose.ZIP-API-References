---
title: "SevenZipArchiveEntry"
second_title: "Aspose.ZIP för Java API-referens"
description: "Representerar en enskild fil i ett 7z-arkiv."
type: docs
weight: 105
url: /sv/java/com.aspose.zip/sevenziparchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class SevenZipArchiveEntry implements IArchiveFileEntry
```

Representerar en enskild fil i ett 7z-arkiv.

Kasta en [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry)-instans till [SevenZipArchiveEntryEncrypted](../../com.aspose.zip/sevenziparchiveentryencrypted) för att avgöra om posten är krypterad eller inte.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extraherar posten till den angivna strömmen. |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | Extraherar posten till den angivna strömmen. |
| [extract(String path)](#extract-java.lang.String-) | Extraherar posten till filsystemet enligt den angivna sökvägen. |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | Extraherar posten till filsystemet enligt den angivna sökvägen. |
| [getCompressedSize()](#getCompressedSize--) | Hämtar storleken på den komprimerade filen. |
| [getCompressionProgressed()](#getCompressionProgressed--) | Hämtar en händelse som utlöses när en del av den råa strömmen komprimeras. |
| [getCompressionSettings()](#getCompressionSettings--) | Hämtar inställningar för komprimering eller dekomprimering. |
| [getLength()](#getLength--) | Hämtar längd. |
| [getModificationTime()](#getModificationTime--) | Hämtar senaste ändringsdatum och -tid. |
| [getName()](#getName--) | Hämtar namnet på posten i arkivet. |
| [getUncompressedSize()](#getUncompressedSize--) | Hämtar storleken på den ursprungliga filen. |
| [isDirectory()](#isDirectory--) | Hämtar ett värde som indikerar om posten representerar en katalog. |
| [open()](#open--) | Öppnar posten för extrahering och tillhandahåller en ström med postens innehåll. |
| [open(String password)](#open-java.lang.String-) | Öppnar posten för extrahering och tillhandahåller en ström med postens innehåll. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Ställer in en händelse som utlöses när en del av den råa strömmen komprimeras. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extraherar posten till den angivna strömmen.

Extrahera en post i zip‑arkivet med lösenord.

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| mål | java.io.OutputStream | destinationsström. Måste vara skrivbar |
| lösenord | java.lang.String | valfritt lösenord för dekryptering |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extraherar posten till filsystemet enligt den angivna sökvägen.

```

``````

try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
archive.getEntries().get(0).extract("data.bin");
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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| path | java.lang.String | sökvägen till destinationsfilen. Om filen redan finns kommer den att skrivas över. |
| lösenord | java.lang.String | valfritt lösenord för dekryptering |

**Returns:**
java.io.File - filinformationen för den extraherade filen
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Hämtar storleken på den komprimerade filen.

**Returns:**
long - storleken på den komprimerade filen
### getCompressionProgressed() {#getCompressionProgressed--}
```
public final Event<ProgressEventArgs> getCompressionProgressed()
```


Hämtar en händelse som utlöses när en del av den råa strömmen komprimeras.

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

Läs från strömmen för att få filens ursprungliga innehåll. Se avsnittet exempel.

**Returns:**
java.io.InputStream - strömmen som representerar innehållet i posten
### open(String password) {#open-java.lang.String-}
```
public final InputStream open(String password)
```


Öppnar posten för extrahering och tillhandahåller en ström med postens innehåll.

Användning:

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

Händelseavsändaren är en [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry)-instans.

Anropas inte i solid läge och i flertrådat läge för LZMA2-poster.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | en händelse som utlöses när en del av den råa strömmen komprimeras |

