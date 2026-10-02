---
title: "TarEntry"
second_title: "Aspose.ZIP för Java API-referens"
description: "Representerar en enskild fil i tar-arkivet."
type: docs
weight: 126
url: /sv/java/com.aspose.zip/tarentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class TarEntry implements IArchiveFileEntry
```

Representerar en enskild fil i tar-arkivet.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extraherar posten till den angivna strömmen. |
| [extract(String path)](#extract-java.lang.String-) | Extraherar posten till filsystemet enligt den angivna sökvägen. |
| [getLength()](#getLength--) | Hämtar längden på posten i byte. |
| [getModificationTime()](#getModificationTime--) | Hämtar ändringstiden för filen eller katalogen. |
| [getName()](#getName--) | Hämtar namnet på posten i arkivet. |
| [getUncompressedSize()](#getUncompressedSize--) | Hämtar storleken på den ursprungliga filen. |
| [isDirectory()](#isDirectory--) | Hämtar ett värde som indikerar om posten representerar en katalog. |
| [open()](#open--) | Öppnar posten för extrahering och tillhandahåller en ström med postens innehåll. |
| [setName(String value)](#setName-java.lang.String-) | Ställer in namnet på posten i arkivet. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extraherar posten till den angivna strömmen.

Extrahera en post från tar-arkivet.

```

``````

try (TarArchive archive = new TarArchive("archive.tar")) {
archive.getEntries().get_Item(0).extract(httpResponseStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | Destination stream. Must be writable. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the entry to the filesystem by the path provided.

```

``````

     try (TarArchive archive = new TarArchive("archive.tar")) {
         archive.getEntries().get_Item(0).extract("data.bin");
     }
 
```



**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| path | java.lang.String | sökvägen till destinationsfilen. Om filen redan finns kommer den att skrivas över. |

**Returns:**
java.io.File - filinformationen för den extraherade filen
### getLength() {#getLength--}
```
public final Long getLength()
```


Hämtar längden på posten i byte.

**Returns:**
java.lang.Long - längden på posten i byte
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Hämtar ändringstiden för filen eller katalogen.

**Returns:**
java.util.Date - modifieringstiden för filen eller katalogen.
### getName() {#getName--}
```
public final String getName()
```


Hämtar namnet på posten i arkivet.

**Returns:**
java.lang.String – namnet på posten i arkivet
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Hämtar storleken på den ursprungliga filen.

Har samma värde som `Length`([getLength](../../com.aspose.zip/tarentry\#getLength--))

**Returns:**
long - storleken på den ursprungliga filen.
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Hämtar ett värde som indikerar om posten representerar en katalog.

**Returns:**
boolean - ett värde som indikerar om posten representerar en katalog
### open() {#open--}
```
public final InputStream open()
```


Öppnar posten för extrahering och tillhandahåller en ström med postens innehåll.


Användning:

```

``````

InputStream decompressed = entry.open();
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
fileStream.write(buffer, 0, bytesRead);
}
 
```

Read from the stream to get the original content of the file. See examples section.

**Returns:**
java.io.InputStream - the stream that represents the contents of the entry
### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Sets the name of the entry within the archive.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the name of the entry within the archive |

