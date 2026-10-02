---
title: "LzxArchiveEntry"
second_title: "Aspose.ZIP för Java API-referens"
description: "Representerar en enskild fil i ett LZX-arkiv."
type: docs
weight: 90
url: /sv/java/com.aspose.zip/lzxarchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class LzxArchiveEntry implements IArchiveFileEntry
```

Representerar en enskild fil i ett LZX-arkiv.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extraherar posten till den angivna strömmen. |
| [extract(String path)](#extract-java.lang.String-) | Extraherar Lzx-arkivinlägg till ett filsystem via sökväg. |
| [getCommentary()](#getCommentary--) | Hämtar kommentaren. |
| [getCompressedSize()](#getCompressedSize--) | Hämtar storleken på den komprimerade filen. |
| [getLength()](#getLength--) | Hämtar längden på posten i byte. |
| [getModificationTime()](#getModificationTime--) | Hämtar den senaste ändringstiden för posten. |
| [getName()](#getName--) | Hämtar postens namn. |
| [getUncompressedSize()](#getUncompressedSize--) | Hämtar storlek på den ursprungliga filen. |
| [isDirectory()](#isDirectory--) | Hämtar ett värde som indikerar om denna post är en katalog. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extraherar posten till den angivna strömmen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| mål | java.io.OutputStream | Destinationsström. Måste vara skrivbar. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extraherar Lzx-arkivinlägg till ett filsystem via sökväg.

```

``````

try (FileInputStream lzxFile = new FileInputStream("archive.lzx")) {
try (LzxArchive archive = new LzxArchive(lzxFile)) {
archive.getEntries().get(0).extract("extracted.bin");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | Path to file which will store decompressed data. |

**Returns:**
java.io.File - FileSystemInfoInstance containing extracted data.
### getCommentary() {#getCommentary--}
```
public final String getCommentary()
```


Gets the commentary.

**Returns:**
java.lang.String - the commentary.
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Gets size of the compressed file.

**Returns:**
long - size of the compressed file.
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets the length of the entry in bytes.

**Returns:**
java.lang.Long - the length of the entry in bytes
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Gets the last modified time of the entry.

**Returns:**
java.util.Date - the last modified time of the entry.
### getName() {#getName--}
```
public final String getName()
```


Gets the name of the entry.

Archives for compression only, such as gzip, bzip2, lzip, lzma, xz, z has name "File.bin" unless another name can be found in headers.

**Returns:**
java.lang.String - the name of the entry
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets size of the original file.

**Returns:**
long - size of the original file.
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Gets a value indicating whether this entry is a directory.

**Returns:**
boolean - a value indicating whether this entry is a directory.
