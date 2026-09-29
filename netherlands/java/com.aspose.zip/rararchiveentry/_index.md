---
title: "RarArchiveEntry"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Stelt een enkel bestand binnen het archief voor."
type: docs
weight: 98
url: /nl/java/com.aspose.zip/rararchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class RarArchiveEntry implements IArchiveFileEntry
```

Stelt een enkel bestand binnen het archief voor.

Cast een [RarArchiveEntry](../../com.aspose.zip/rararchiveentry) instantie naar [RarArchiveEntryEncrypted](../../com.aspose.zip/rararchiveentryencrypted) om te bepalen of het item versleuteld is of niet.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extraheert het item naar de opgegeven stream. |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | Extraheert het item naar de opgegeven stream. |
| [extract(String path)](#extract-java.lang.String-) | Extraheert het item naar het bestandssysteem via het opgegeven pad. |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | Extraheert het item naar het bestandssysteem via het opgegeven pad. |
| [getCompressedSize()](#getCompressedSize--) | Haalt de grootte van het gecomprimeerde bestand op. |
| [getCreationTime()](#getCreationTime--) | Haalt de aanmaakdatum en -tijd op. |
| [getExtractionProgressed()](#getExtractionProgressed--) | Haalt een gebeurtenis op die wordt opgegeven wanneer een deel van de ruwe stream wordt geëxtraheerd. |
| [getLastAccessTime()](#getLastAccessTime--) | Haalt de datum en tijd van laatste toegang op. |
| [getLength()](#getLength--) | Haalt de lengte op. |
| [getModificationTime()](#getModificationTime--) | Haalt de datum en tijd van de laatste wijziging op. |
| [getName()](#getName--) | Haalt de naam van het item binnen het archief op. |
| [getUncompressedSize()](#getUncompressedSize--) | Haalt de grootte van het originele bestand op. |
| [isDirectory()](#isDirectory--) | Haalt een waarde op die aangeeft of het item een map vertegenwoordigt. |
| [open()](#open--) | Opent het item voor extractie en levert een stream met gedecomprimeerde inhoud van het item. |
| [open(String password)](#open-java.lang.String-) | Opent het item voor extractie en levert een stream met gedecomprimeerde inhoud van het item. |
| [setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Stelt een gebeurtenis in die wordt opgegeven wanneer een deel van de ruwe stream wordt geëxtraheerd. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extraheert het item naar de opgegeven stream.


Extraheer een item uit een rar-archief met wachtwoord.

```

``````

try (FileInputStream rarFile = new FileInputStream(\"archive.rar\")) {
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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| bestemming | java.io.OutputStream | Doelstream. Moet beschrijfbaar zijn. |
| password | java.lang.String | Optioneel wachtwoord voor ontcijfering. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extraheert het item naar het bestandssysteem via het opgegeven pad.


Extraheer twee items uit een rar-archief.

```

``````

try (FileInputStream rarFile = new FileInputStream(\"archive.rar\")) {
try (RarArchive archive = new RarArchive(rarFile)) {
archive.getEntries().get(0).extract(\"first.bin\", \"pass\");
archive.getEntries().get(1).extract(\"second.bin\", \"pass\");
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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | Het pad naar het doelbestand. Als het bestand al bestaat, wordt het overschreven. |
| password | java.lang.String | Optioneel wachtwoord voor ontcijfering. |

**Returns:**
java.io.File - de bestandsinformatie van het geëxtraheerde bestand
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Haalt de grootte van het gecomprimeerde bestand op.

**Returns:**
long - de grootte van het gecomprimeerde bestand
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


Haalt de aanmaakdatum en -tijd op.

**Returns:**
java.util.Date - aanmaakdatum en -tijd.
### getExtractionProgressed() {#getExtractionProgressed--}
```
public final Event<ProgressEventArgs> getExtractionProgressed()
```


Haalt een gebeurtenis op die wordt opgegeven wanneer een deel van de ruwe stream wordt geëxtraheerd.

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

Lees van de stream om de oorspronkelijke inhoud van het bestand te krijgen. Zie de sectie voorbeelden.

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

Event-afzender is een [RarArchiveEntry](../../com.aspose.zip/rararchiveentry) instantie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | een gebeurtenis die wordt opgehaald wanneer een deel van de ruwe stream is geëxtraheerd. |

