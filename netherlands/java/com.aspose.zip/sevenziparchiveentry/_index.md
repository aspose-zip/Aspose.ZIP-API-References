---
title: "SevenZipArchiveEntry"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Vertegenwoordigt een enkel bestand binnen een 7z-archief."
type: docs
weight: 105
url: /nl/java/com.aspose.zip/sevenziparchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class SevenZipArchiveEntry implements IArchiveFileEntry
```

Vertegenwoordigt een enkel bestand binnen een 7z-archief.

Cast een [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) exemplaar naar [SevenZipArchiveEntryEncrypted](../../com.aspose.zip/sevenziparchiveentryencrypted) om te bepalen of het item versleuteld is of niet.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extraheert het item naar de opgegeven stream. |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | Extraheert het item naar de opgegeven stream. |
| [extract(String path)](#extract-java.lang.String-) | Extraheert het item naar het bestandssysteem via het opgegeven pad. |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | Extraheert het item naar het bestandssysteem via het opgegeven pad. |
| [getCompressedSize()](#getCompressedSize--) | Haalt de grootte van het gecomprimeerde bestand op. |
| [getCompressionProgressed()](#getCompressionProgressed--) | Haalt een gebeurtenis op die wordt geactiveerd wanneer een deel van de ruwe stream wordt gecomprimeerd. |
| [getCompressionSettings()](#getCompressionSettings--) | Haalt instellingen op voor compressie of decompressie. |
| [getLength()](#getLength--) | Haalt de lengte op. |
| [getModificationTime()](#getModificationTime--) | Haalt de datum en tijd van de laatste wijziging op. |
| [getName()](#getName--) | Haalt de naam van het item binnen het archief op. |
| [getUncompressedSize()](#getUncompressedSize--) | Haalt de grootte van het originele bestand op. |
| [isDirectory()](#isDirectory--) | Haalt een waarde op die aangeeft of het item een map vertegenwoordigt. |
| [open()](#open--) | Opent het item voor extractie en levert een stream met de inhoud van het item. |
| [open(String password)](#open-java.lang.String-) | Opent het item voor extractie en levert een stream met de inhoud van het item. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Stelt een gebeurtenis in die wordt geactiveerd wanneer een deel van de ruwe stream wordt gecomprimeerd. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extraheert het item naar de opgegeven stream.

Extraheer een item uit een zip-archief met wachtwoord.

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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| bestemming | java.io.OutputStream | doelstream. Moet beschrijfbaar zijn. |
| password | java.lang.String | optioneel wachtwoord voor ontcijfering |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extraheert het item naar het bestandssysteem via het opgegeven pad.

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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | het pad naar het bestemmingsbestand. Als het bestand al bestaat, wordt het overschreven |
| password | java.lang.String | optioneel wachtwoord voor ontcijfering |

**Returns:**
java.io.File - de bestandsinformatie van het geëxtraheerde bestand
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Haalt de grootte van het gecomprimeerde bestand op.

**Returns:**
long - de grootte van het gecomprimeerde bestand
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

Lees van de stream om de oorspronkelijke inhoud van het bestand te krijgen. Zie de sectie voorbeelden.

**Returns:**
java.io.InputStream - de stream die de inhoud van het item vertegenwoordigt
### open(String password) {#open-java.lang.String-}
```
public final InputStream open(String password)
```


Opent het item voor extractie en levert een stream met de inhoud van het item.

Gebruik:

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

Eventzender is een [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) instantie.

Wordt niet aangeroepen in solid-modus en in multithread-modus voor LZMA2-items.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | een gebeurtenis die wordt opgehaald wanneer een deel van de ruwe stream wordt gecomprimeerd |

