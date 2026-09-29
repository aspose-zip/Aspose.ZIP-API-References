---
title: "LhaArchiveEntry"
second_title: "Aspose.ZIP för Java API-referens"
description: "Representerar en enskild fil i ett Lha-arkiv."
type: docs
weight: 76
url: /sv/java/com.aspose.zip/lhaarchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class LhaArchiveEntry implements IArchiveFileEntry
```

Representerar en enskild fil i ett Lha-arkiv.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [extract(File file)](#extract-java.io.File-) | Extraherar Lha-arkivpost till en fil. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extraherar posten till den angivna strömmen. |
| [extract(String path)](#extract-java.lang.String-) | Extraherar Lha-arkivpost till ett filsystem enligt sökväg. |
| [getLastModified()](#getLastModified--) | Hämtar den senaste ändringstiden för posten. |
| [getLength()](#getLength--) | Hämtar längden på posten i byte. |
| [getModificationTime()](#getModificationTime--) | Hämtar den senaste ändringstiden för posten. |
| [getName()](#getName--) | Hämtar postens namn. |
| [getPath()](#getPath--) | Hämtar hela sökvägen till posten. |
| [isDirectory()](#isDirectory--) | Hämtar ett värde som indikerar om denna post är en katalog. |
### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Extraherar Lha-arkivpost till en fil.

```

``````

try (FileInputStream lhaFile = new FileInputStream("archive.lha")) {
try (LhaArchive archive = new LhaArchive(lhaFile)) {
archive.getEntries().get(0).extract(new File("extracted.bin"));
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | File for storing decompressed data.

Does nothing for directory entry |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts the entry to the stream provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts Lha archive entry to a filesystem by path.

```

``````

     try (FileInputStream lhaFile = new FileInputStream("archive.lha")) {
         try (LhaArchive archive = new LhaArchive(lhaFile)) {
             archive.getEntries().get(0).extract("extracted.bin");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| path | java.lang.String | sökvägen till filen som kommer att lagra dekomprimerad data |

**Returns:**
java.io.File - java.io.File-instans som innehåller extraherade data
### getLastModified() {#getLastModified--}
```
public final Date getLastModified()
```


Hämtar den senaste ändringstiden för posten.

**Returns:**
java.util.Date - den senaste ändringstiden för posten
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


Hämtar den senaste ändringstiden för posten.

**Returns:**
java.util.Date - den senaste ändringstiden för posten
### getName() {#getName--}
```
public final String getName()
```


Hämtar postens namn.

Arkiv endast för komprimering, såsom gzip, bzip2, lzip, lzma, xz, z har namnet "File.bin" om inte ett annat namn kan hittas i rubrikerna.

**Returns:**
java.lang.String - postens namn
### getPath() {#getPath--}
```
public final String getPath()
```


Hämtar hela sökvägen till posten.

**Returns:**
java.lang.String - hela sökvägen till posten
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Hämtar ett värde som indikerar om denna post är en katalog.

**Returns:**
boolean - ett värde som indikerar om denna post är en katalog.
