---
title: "ArchiveEntry"
second_title: "Aspose.ZIP för Java API-referens"
description: "Representerar en enskild fil i arkivet."
type: docs
weight: 27
url: /sv/java/com.aspose.zip/archiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class ArchiveEntry implements IArchiveFileEntry
```

Representerar en enskild fil i arkivet.

Kasta en [ArchiveEntry](../../com.aspose.zip/archiveentry)-instans till [ArchiveEntryEncrypted](../../com.aspose.zip/archiveentryencrypted) för att avgöra om posten är krypterad eller inte.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extraherar posten till den angivna strömmen. |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | Extraherar posten till den angivna strömmen. |
| [extract(String path)](#extract-java.lang.String-) | Extraherar posten till filsystemet enligt den angivna sökvägen. |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | Extraherar posten till filsystemet enligt den angivna sökvägen. |
| [getComment()](#getComment--) | Hämtar kommentaren för posten i arkivet. |
| [getCompressedSize()](#getCompressedSize--) | Hämtar storleken på den komprimerade filen. |
| [getCompressionProgressed()](#getCompressionProgressed--) | Hämtar en händelse som utlöses när en del av den råa strömmen komprimeras. |
| [getCompressionSettings()](#getCompressionSettings--) | Hämtar inställningar för komprimering eller dekomprimering. |
| [getDataSource()](#getDataSource--) | Källa för posten om posten lades till i arkivet, inte extraherades. |
| [getExtractionProgressed()](#getExtractionProgressed--) | Hämtar en händelse som utlöses när en del av råströmmen har extraherats. |
| [getLength()](#getLength--) | Hämtar längd. |
| [getModificationTime()](#getModificationTime--) | Hämtar senaste ändringsdatum och -tid. |
| [getName()](#getName--) | Hämtar namn på posten i arkivet. |
| [getUncompressedSize()](#getUncompressedSize--) | Hämtar storlek på den ursprungliga filen. |
| [isDirectory()](#isDirectory--) | Hämtar ett värde som indikerar om posten representerar en katalog. |
| [open()](#open--) | Öppnar posten för extraktion och tillhandahåller en ström med dekomprimerat postinnehåll. |
| [open(String password)](#open-java.lang.String-) | Öppnar posten för extraktion och tillhandahåller en ström med dekomprimerat postinnehåll. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Ställer in en händelse som utlöses när en del av den råa strömmen komprimeras. |
| [setExtractionProgressed(Event&lt;ProgressCancelEventArgs&gt; value)](#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressCancelEventArgs--) | Ställer in en händelse som utlöses när en del av råströmmen har extraherats. |
| [setModificationTime(Date value)](#setModificationTime-java.util.Date-) | Ställer in senaste ändringsdatum och -tid. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extraherar posten till den angivna strömmen.

Extrahera en post i zip‑arkivet med lösenord.

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| mål | java.io.OutputStream | Destinationsström. Måste vara skrivbar. |
| lösenord | java.lang.String | Valfritt lösenord för dekryptering. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extraherar posten till filsystemet enligt den angivna sökvägen.

Extrahera två poster i ZIP‑arkivet, var och en med eget lösenord.

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| path | java.lang.String | Sökvägen till destinationsfilen. Om filen redan finns kommer den att skrivas över. |
| lösenord | java.lang.String | Valfritt lösenord för dekryptering. |

**Returns:**
java.io.File - filinformationen för den extraherade filen
### getComment() {#getComment--}
```
public final String getComment()
```


Hämtar kommentaren för posten i arkivet.

**Returns:**
java.lang.String - kommentar för posten i arkivet
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Hämtar storleken på den komprimerade filen.

**Returns:**
long - storlek på den komprimerade filen
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

I det här exemplet används händelsehanteraren för avbrytning efter att de första hundra Mb av posten har extraherats.

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

Läs från strömmen för att få filens ursprungliga innehåll.

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

Avsändaren för händelsen är en [ArchiveEntry](../../com.aspose.zip/archiveentry) instans.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | en händelse som utlöses när en del av den råa strömmen komprimeras |

### setExtractionProgressed(Event&lt;ProgressCancelEventArgs&gt; value) {#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressCancelEventArgs--}
```
public final void setExtractionProgressed(Event<ProgressCancelEventArgs> value)
```


Ställer in en händelse som utlöses när en del av råströmmen har extraherats.

I det här exemplet används händelsehanteraren för att beräkna andelen av den behandlade storleken i procent.

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

Avsändaren för händelsen är en [ArchiveEntry](../../com.aspose.zip/archiveentry) instans. Det är möjligt att avbryta extraheringen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | com.aspose.zip.Event&lt;com.aspose.zip.ProgressCancelEventArgs&gt; | en händelse som utlöses när en del av den råa strömmen har extraherats. |

### setModificationTime(Date value) {#setModificationTime-java.util.Date-}
```
public final void setModificationTime(Date value)
```


Ställer in senaste ändringsdatum och -tid.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Date | senast ändrade datum och tid |

