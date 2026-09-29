---
title: "CpioEntry"
second_title: "Aspose.ZIP för Java API-referens"
description: "Representerar en enskild fil i ett cpio-arkiv."
type: docs
weight: 58
url: /sv/java/com.aspose.zip/cpioentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public final class CpioEntry implements IArchiveFileEntry
```

Representerar en enskild fil i ett cpio-arkiv.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extraherar posten till den angivna strömmen. |
| [extract(String path)](#extract-java.lang.String-) | Extraherar posten till filsystemet enligt den angivna sökvägen. |
| [getLastWriteTimeUtc()](#getLastWriteTimeUtc--) | Hämtar den senaste skrivtiden. |
| [getLength()](#getLength--) | Hämtar längden på posten i byte. |
| [getName()](#getName--) | Hämtar namnet på posten i arkivet. |
| [getParent()](#getParent--) | Hämtar arkivet som posten tillhör. |
| [isDirectory()](#isDirectory--) | Hämtar ett värde som indikerar om posten representerar en katalog. |
| [open()](#open--) | Öppnar posten för extrahering och tillhandahåller en ström med postens innehåll. |
| [toString()](#toString--) | Returnerar en strängrepresentation av instansen av klassen [CpioEntry](../../com.aspose.zip/cpioentry). |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extraherar posten till den angivna strömmen.

Extrahera en post från cpio-arkivet.

```

``````

try (CpioArchive archive = new CpioArchive("archive.cpio")) {
archive.getEntries().get(0).extract(httpResponseStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream. Must be writable |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the entry to the filesystem by the path provided.

```

``````

     try (CpioArchive archive = new CpioArchive("archive.cpio")) {
         archive.getEntries().get(0).extract("data.bin");
     }
 
```



**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| path | java.lang.String | sökvägen till destinationsfilen. Om filen redan finns kommer den att skrivas över. |

**Returns:**
java.io.File - filinformationen för den extraherade filen
### getLastWriteTimeUtc() {#getLastWriteTimeUtc--}
```
public final Date getLastWriteTimeUtc()
```


Hämtar den senaste skrivtiden.

**Returns:**
java.util.Date – den senaste skrivtiden
### getLength() {#getLength--}
```
public final Long getLength()
```


Hämtar längden på posten i byte.

**Returns:**
java.lang.Long - längden på posten i byte
### getName() {#getName--}
```
public final String getName()
```


Hämtar namnet på posten i arkivet.

**Returns:**
java.lang.String – namnet på posten i arkivet
### getParent() {#getParent--}
```
public final CpioArchive getParent()
```


Hämtar arkivet som posten tillhör.

**Returns:**
[CpioArchive](../../com.aspose.zip/cpioarchive) - the archive the entry belongs to
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Hämtar ett värde som indikerar om posten representerar en katalog.

**Returns:**
boolean – ett värde som indikerar om posten representerar en katalog.
### open() {#open--}
```
public final InputStream open()
```


Öppnar posten för extrahering och tillhandahåller en ström med postens innehåll.

Användning:

```

``````

CpioArchive archive = new CpioArchive("archive.cpio");
CpioEntry entry = archive.getEntries().get(0);
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

Read from the stream to get the original content of a file. See examples section.

**Returns:**
java.io.InputStream - the stream that represents the contents of the entry
### toString() {#toString--}
```
public String toString()
```


Returns string representation of the instance of the [CpioEntry](../../com.aspose.zip/cpioentry) class.

**Returns:**
java.lang.String - string representation of this object.
