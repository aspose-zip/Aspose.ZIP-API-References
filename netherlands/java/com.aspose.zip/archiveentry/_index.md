---
title: "ArchiveEntry"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Stelt een enkel bestand binnen het archief voor."
type: docs
weight: 27
url: /nl/java/com.aspose.zip/archiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class ArchiveEntry implements IArchiveFileEntry
```

Stelt een enkel bestand binnen het archief voor.

Cast een [ArchiveEntry](../../com.aspose.zip/archiveentry) instantie naar [ArchiveEntryEncrypted](../../com.aspose.zip/archiveentryencrypted) om te bepalen of de entry versleuteld is of niet.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extraheert het item naar de opgegeven stream. |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | Extraheert het item naar de opgegeven stream. |
| [extract(String path)](#extract-java.lang.String-) | Extraheert het item naar het bestandssysteem via het opgegeven pad. |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | Extraheert het item naar het bestandssysteem via het opgegeven pad. |
| [getComment()](#getComment--) | Haalt de opmerking van de entry binnen het archief op. |
| [getCompressedSize()](#getCompressedSize--) | Haalt de grootte van het gecomprimeerde bestand op. |
| [getCompressionProgressed()](#getCompressionProgressed--) | Haalt een gebeurtenis op die wordt geactiveerd wanneer een deel van de ruwe stream wordt gecomprimeerd. |
| [getCompressionSettings()](#getCompressionSettings--) | Haalt instellingen op voor compressie of decompressie. |
| [getDataSource()](#getDataSource--) | Bron voor de entry als de entry aan het archief is toegevoegd, niet geëxtraheerd. |
| [getExtractionProgressed()](#getExtractionProgressed--) | Haalt een gebeurtenis op die wordt opgegeven wanneer een deel van de ruwe stream wordt geëxtraheerd. |
| [getLength()](#getLength--) | Haalt de lengte op. |
| [getModificationTime()](#getModificationTime--) | Haalt de datum en tijd van de laatste wijziging op. |
| [getName()](#getName--) | Haalt de naam van het item binnen het archief op. |
| [getUncompressedSize()](#getUncompressedSize--) | Haalt de grootte van het oorspronkelijke bestand op. |
| [isDirectory()](#isDirectory--) | Haalt een waarde op die aangeeft of het item een map vertegenwoordigt. |
| [open()](#open--) | Opent het item voor extractie en levert een stream met gedecomprimeerde inhoud van het item. |
| [open(String password)](#open-java.lang.String-) | Opent het item voor extractie en levert een stream met gedecomprimeerde inhoud van het item. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Stelt een gebeurtenis in die wordt geactiveerd wanneer een deel van de ruwe stream wordt gecomprimeerd. |
| [setExtractionProgressed(Event&lt;ProgressCancelEventArgs&gt; value)](#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressCancelEventArgs--) | Stelt een gebeurtenis in die wordt opgegeven wanneer een deel van de ruwe stream wordt geëxtraheerd. |
| [setModificationTime(Date value)](#setModificationTime-java.util.Date-) | Stelt de datum en tijd van laatste wijziging in. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extraheert het item naar de opgegeven stream.

Extraheer een item uit een zip-archief met wachtwoord.

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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| bestemming | java.io.OutputStream | Doelstream. Moet beschrijfbaar zijn. |
| password | java.lang.String | Optioneel wachtwoord voor ontcijfering. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extraheert het item naar het bestandssysteem via het opgegeven pad.

Extraheer twee items uit een ZIP-archief, elk met een eigen wachtwoord.

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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | Het pad naar het doelbestand. Als het bestand al bestaat, wordt het overschreven. |
| password | java.lang.String | Optioneel wachtwoord voor ontcijfering. |

**Returns:**
java.io.File - de bestandsinformatie van het geëxtraheerde bestand
### getComment() {#getComment--}
```
public final String getComment()
```


Haalt de opmerking van de entry binnen het archief op.

**Returns:**
java.lang.String - commentaar van het item binnen het archief
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Haalt de grootte van het gecomprimeerde bestand op.

**Returns:**
long - grootte van het gecomprimeerde bestand
### getCompressionProgressed() {#getCompressionProgressed--}
```
public final Event<ProgressEventArgs> getCompressionProgressed()
```


Haalt een gebeurtenis op die wordt geactiveerd wanneer een deel van de ruwe stream wordt gecomprimeerd.

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

In dit voorbeeld wordt de gebeurtenishandler gebruikt voor annulering nadat de eerste honderd MB van het item is geëxtraheerd.

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

Lees van de stream om de oorspronkelijke inhoud van het bestand te krijgen.

**Returns:**
java.io.InputStream - De stream die de inhoud van het item vertegenwoordigt.
### open(String password) {#open-java.lang.String-}
```
public final InputStream open(String password)
```


Opent het item voor extractie en levert een stream met gedecomprimeerde inhoud van het item.


Gebruik:

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

Eventzender is een [ArchiveEntry](../../com.aspose.zip/archiveentry) instantie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | een gebeurtenis die wordt opgehaald wanneer een deel van de ruwe stream wordt gecomprimeerd |

### setExtractionProgressed(Event&lt;ProgressCancelEventArgs&gt; value) {#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressCancelEventArgs--}
```
public final void setExtractionProgressed(Event<ProgressCancelEventArgs> value)
```


Stelt een gebeurtenis in die wordt opgegeven wanneer een deel van de ruwe stream wordt geëxtraheerd.

In dit voorbeeld wordt de gebeurtenishandler gebruikt om het aandeel van de verwerkte grootte in procenten te berekenen.

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

Eventzender is een [ArchiveEntry](../../com.aspose.zip/archiveentry) instantie. Het is mogelijk om extractie te annuleren.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | com.aspose.zip.Event&lt;com.aspose.zip.ProgressCancelEventArgs&gt; | een gebeurtenis die wordt opgehaald wanneer een deel van de ruwe stream is geëxtraheerd. |

### setModificationTime(Date value) {#setModificationTime-java.util.Date-}
```
public final void setModificationTime(Date value)
```


Stelt de datum en tijd van laatste wijziging in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.Date | laatste wijzigingsdatum en -tijd |

