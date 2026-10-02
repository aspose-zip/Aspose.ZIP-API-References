---
title: "ArjEntryPlain"
second_title: "Aspose.ZIP för Java API-referens"
description: "Representerar en enskild fil i ett ARJ-arkiv."
type: docs
weight: 38
url: /sv/java/com.aspose.zip/arjentryplain/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class ArjEntryPlain implements IArchiveFileEntry
```

Representerar en enskild fil i ett ARJ-arkiv.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [extract(File file)](#extract-java.io.File-) | Extraherar en ARJ-arkivpost till en fil. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extraherar posten till den angivna strömmen. |
| [extract(String path)](#extract-java.lang.String-) | Extraherar posten till filsystemet enligt den angivna sökvägen. |
| [getCompressedSize()](#getCompressedSize--) | Hämtar storleken på den komprimerade filen. |
| [getLength()](#getLength--) | Hämtar längden på posten i byte. |
| [getName()](#getName--) | Hämtar namn på posten i arkivet. |
| [getUncompressedSize()](#getUncompressedSize--) | Hämtar storlek på den ursprungliga filen. |
### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Extraherar en ARJ-arkivpost till en fil.

```

``````

try (FileInputStream arjFile = new FileInputStream("sourceFileName")) {
try (ArjArchive archive = new ArjArchive(arjFile)) {
archive.getEntries().get(0).extract(new File("extracted.bin"));
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | java.io.File for storing decompressed data |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts the entry to the stream provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | Destination stream. Must be writable. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the entry to the filesystem by the path provided.

Extract two entries of rar archive.

```

``````

     try (FileInputStream arjFile = new FileInputStream("archive.arj")) {
         try (ArjArchive archive = new ArjArchive(arjFile)) {
             archive.getEntries().get(0).extract("first.bin");
             archive.getEntries().get(1).extract("second.bin");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| path | java.lang.String | sökvägen till destinationsfilen. Om filen redan finns kommer den att skrivas över. |

**Returns:**
java.io.File - filinformationen för den sammansatta filen
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Hämtar storleken på den komprimerade filen.

**Returns:**
long - storleken på den komprimerade filen
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


Hämtar namn på posten i arkivet.

**Returns:**
java.lang.String - namn på posten i arkivet
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Hämtar storlek på den ursprungliga filen.

**Returns:**
long - storlek på den ursprungliga filen
