---
title: "CpioEntry"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Vertegenwoordigt een enkel bestand binnen een cpio-archief."
type: docs
weight: 58
url: /nl/java/com.aspose.zip/cpioentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public final class CpioEntry implements IArchiveFileEntry
```

Vertegenwoordigt een enkel bestand binnen een cpio-archief.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extraheert het item naar de opgegeven stream. |
| [extract(String path)](#extract-java.lang.String-) | Extraheert het item naar het bestandssysteem via het opgegeven pad. |
| [getLastWriteTimeUtc()](#getLastWriteTimeUtc--) | Haalt de laatste schrijftijd op. |
| [getLength()](#getLength--) | Haalt de lengte van het item op in bytes. |
| [getName()](#getName--) | Haalt de naam van het item binnen het archief op. |
| [getParent()](#getParent--) | Haalt het archief op waartoe het item behoort. |
| [isDirectory()](#isDirectory--) | Haalt een waarde op die aangeeft of het item een map vertegenwoordigt. |
| [open()](#open--) | Opent het item voor extractie en levert een stream met de inhoud van het item. |
| [toString()](#toString--) | Retourneert de tekenreeksrepresentatie van het exemplaar van de klasse [CpioEntry](../../com.aspose.zip/cpioentry). |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extraheert het item naar de opgegeven stream.

Extraheer een item uit een cpio-archief.

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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | het pad naar het bestemmingsbestand. Als het bestand al bestaat, wordt het overschreven |

**Returns:**
java.io.File - de bestandsinformatie van het geëxtraheerde bestand
### getLastWriteTimeUtc() {#getLastWriteTimeUtc--}
```
public final Date getLastWriteTimeUtc()
```


Haalt de laatste schrijftijd op.

**Returns:**
java.util.Date - de laatste schrijftijd
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
java.lang.String - de naam van het item binnen het archief
### getParent() {#getParent--}
```
public final CpioArchive getParent()
```


Haalt het archief op waartoe het item behoort.

**Returns:**
[CpioArchive](../../com.aspose.zip/cpioarchive) - the archive the entry belongs to
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Haalt een waarde op die aangeeft of het item een map vertegenwoordigt.

**Returns:**
boolean - een waarde die aangeeft of het item een map vertegenwoordigt.
### open() {#open--}
```
public final InputStream open()
```


Opent het item voor extractie en levert een stream met de inhoud van het item.

Gebruik:

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
