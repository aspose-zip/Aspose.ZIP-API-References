---
title: "ArjEntryPlain"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Vertegenwoordigt een enkel bestand binnen een ARJ-archief."
type: docs
weight: 38
url: /nl/java/com.aspose.zip/arjentryplain/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class ArjEntryPlain implements IArchiveFileEntry
```

Vertegenwoordigt een enkel bestand binnen een ARJ-archief.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [extract(File file)](#extract-java.io.File-) | Extraheert een ARJ-archiefitem naar een bestand. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extraheert het item naar de opgegeven stream. |
| [extract(String path)](#extract-java.lang.String-) | Extraheert het item naar het bestandssysteem via het opgegeven pad. |
| [getCompressedSize()](#getCompressedSize--) | Haalt de grootte van het gecomprimeerde bestand op. |
| [getLength()](#getLength--) | Haalt de lengte van het item op in bytes. |
| [getName()](#getName--) | Haalt de naam van het item binnen het archief op. |
| [getUncompressedSize()](#getUncompressedSize--) | Haalt de grootte van het oorspronkelijke bestand op. |
### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Extraheert een ARJ-archiefitem naar een bestand.

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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | het pad naar het bestemmingsbestand. Als het bestand al bestaat, wordt het overschreven |

**Returns:**
java.io.File - de bestandsinformatie van het samengestelde bestand
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Haalt de grootte van het gecomprimeerde bestand op.

**Returns:**
long - de grootte van het gecomprimeerde bestand
### getLength() {#getLength--}
```
public final Long getLength()
```


Haalt de lengte van het item op in bytes.

**Returns:**
java.lang.Long - de lengte van het item in bytes
### getName() {#getName--}
```
public final String getName()
```


Haalt de naam van het item binnen het archief op.

**Returns:**
java.lang.String - naam van het item binnen het archief
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Haalt de grootte van het oorspronkelijke bestand op.

**Returns:**
long - grootte van het originele bestand
