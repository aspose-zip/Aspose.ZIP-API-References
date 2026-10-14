---
title: "AppleArchiveEntry"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Stelt een bestand- of mapvermelding voor binnen een ."
type: docs
weight: 17
url: /nl/java/com.aspose.zip/applearchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public final class AppleArchiveEntry implements IArchiveFileEntry
```

Stelt een bestand- of mapvermelding voor binnen een [AppleArchive](../../com.aspose.zip/applearchive).

Een instantie van deze klasse kan ofwel een vermelding vertegenwoordigen die is geparseerd uit een bestaande Apple Archive of een vermelding die is toegevoegd aan een archief dat wordt samengesteld.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extraheert het item naar de opgegeven stream. |
| [extract(String path)](#extract-java.lang.String-) | Extraheert Apple-archiefvermelding naar een bestandssysteem via pad. |
| [getLength()](#getLength--) | Haalt de ongecomprimeerde lengte van de vermelding op in bytes. |
| [getName()](#getName--) | Haalt het pad van de vermelding op binnen het archief. |
| [isDirectory()](#isDirectory--) | Haalt een waarde op die aangeeft of het item een map vertegenwoordigt. |
| [open()](#open--) | Opent de vermelding voor extractie en levert een stream met de inhoud van de vermelding. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public void extract(OutputStream destination)
```


Extraheert het item naar de opgegeven stream.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| bestemming | java.io.OutputStream | doelstream. Moet beschrijfbaar zijn. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extraheert Apple-archiefvermelding naar een bestandssysteem via pad.

```

``````

try (FileInputStream aaFile = new FileInputStream("archive.aa")) {
try (AppleArchive archive = new AppleArchive(aaFile)) {
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
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets the uncompressed length of the entry in bytes.

For directory entries the value is zero. For entries created from a non-seekable source stream the length can be unknown.

**Returns:**
java.lang.Long - the uncompressed length of the entry in bytes.
### getName() {#getName--}
```
public final String getName()
```


Gets the path of the entry inside the archive.

The value is the archive path recorded for the entry. Directory entries usually end with Forward slash (`/`).

**Returns:**
java.lang.String - the path of the entry inside the archive.
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


Opens the entry for extraction and provides a stream with the entry content.

**Returns:**
java.io.InputStream - A readable stream that contains the extracted entry data.
