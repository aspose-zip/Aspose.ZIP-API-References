---
title: "CabEntry"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Vertegenwoordigt een enkel bestand binnen een cab-archief."
type: docs
weight: 46
url: /nl/java/com.aspose.zip/cabentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public final class CabEntry implements IArchiveFileEntry
```

Vertegenwoordigt een enkel bestand binnen een cab-archief.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extraheert het item naar de opgegeven stream. |
| [extract(String path)](#extract-java.lang.String-) | Extraheert het item naar het bestandssysteem via het opgegeven pad. |
| [getLength()](#getLength--) | Haalt de lengte van het item op in bytes. |
| [getModificationTime()](#getModificationTime--) | Haalt de datum en tijd van de laatste wijziging op. |
| [getName()](#getName--) | Haalt de naam van het item binnen het archief op. |
| [open()](#open--) | Opent het item voor extractie en levert een stream met de inhoud van het item. |
| [toString()](#toString--) | Retourneert de tekenreeksrepresentatie van de instantie van de [CabEntry](../../com.aspose.zip/cabentry) klasse. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extraheert het item naar de opgegeven stream.

Extraheer een item uit een CAB-archief.

```

``````

try (CabArchive archive = new CabArchive("archive.cab")) {
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

     try (CabArchive archive = new CabArchive("archive.cab")) {
         archive.getEntries().get(0).extract("data.bin");
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | het pad naar het bestemmingsbestand. Als het bestand al bestaat, wordt het overschreven |

**Returns:**
java.io.File - de bestandsinformatie van een samengesteld bestand
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


Haalt de datum en tijd van de laatste wijziging op.

**Returns:**
java.util.Date - datum en tijd van laatste wijziging.
### getName() {#getName--}
```
public final String getName()
```


Haalt de naam van het item binnen het archief op.

**Returns:**
java.lang.String - de naam van het item binnen het archief
### open() {#open--}
```
public final InputStream open()
```


Opent het item voor extractie en levert een stream met de inhoud van het item.

Gebruik:

```

``````

CabArchive archive = new CabArchive("archive.cab");
CabEntry entry = archive.getEntries().get(0);
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


Returns string representation of the instance of the [CabEntry](../../com.aspose.zip/cabentry) class.

**Returns:**
java.lang.String - string representation of this object
