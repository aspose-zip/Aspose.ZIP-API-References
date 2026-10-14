---
title: "LhaArchiveEntry"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Vertegenwoordigt een enkel bestand binnen een Lha-archief."
type: docs
weight: 76
url: /nl/java/com.aspose.zip/lhaarchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class LhaArchiveEntry implements IArchiveFileEntry
```

Vertegenwoordigt een enkel bestand binnen een Lha-archief.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [extract(File file)](#extract-java.io.File-) | Extraheert Lha-archiefitem naar een bestand. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extraheert het item naar de opgegeven stream. |
| [extract(String path)](#extract-java.lang.String-) | Extraheert Lha-archiefitem naar een bestandssysteem via pad. |
| [getLastModified()](#getLastModified--) | Haalt de laatst gewijzigde tijd van het item op. |
| [getLength()](#getLength--) | Haalt de lengte van het item op in bytes. |
| [getModificationTime()](#getModificationTime--) | Haalt de laatst gewijzigde tijd van het item op. |
| [getName()](#getName--) | Haalt de naam van het item op. |
| [getPath()](#getPath--) | Haalt het volledige pad naar het item op. |
| [isDirectory()](#isDirectory--) | Haalt een waarde op die aangeeft of dit item een map is. |
### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Extraheert Lha-archiefitem naar een bestand.

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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | het pad naar het bestand dat de gedecomprimeerde gegevens zal opslaan |

**Returns:**
java.io.File - java.io.File‑instantie die geëxtraheerde gegevens bevat
### getLastModified() {#getLastModified--}
```
public final Date getLastModified()
```


Haalt de laatst gewijzigde tijd van het item op.

**Returns:**
java.util.Date - de laatst gewijzigde tijd van het item
### getLength() {#getLength--}
```
public final Long getLength()
```


Haalt de lengte van het item op in bytes.

**Returns:**
java.lang.Long - de lengte van het item in bytes
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Haalt de laatst gewijzigde tijd van het item op.

**Returns:**
java.util.Date - de laatst gewijzigde tijd van het item
### getName() {#getName--}
```
public final String getName()
```


Haalt de naam van het item op.

Archieven alleen voor compressie, zoals gzip, bzip2, lzip, lzma, xz, z, hebben de naam "File.bin" tenzij een andere naam in de headers kan worden gevonden.

**Returns:**
java.lang.String - de naam van de entry
### getPath() {#getPath--}
```
public final String getPath()
```


Haalt het volledige pad naar het item op.

**Returns:**
java.lang.String - het volledige pad naar het item
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Haalt een waarde op die aangeeft of dit item een map is.

**Returns:**
boolean - een waarde die aangeeft of dit item een map is.
