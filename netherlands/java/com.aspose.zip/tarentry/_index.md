---
title: "TarEntry"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Vertegenwoordigt een enkel bestand binnen tar-archief."
type: docs
weight: 126
url: /nl/java/com.aspose.zip/tarentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class TarEntry implements IArchiveFileEntry
```

Vertegenwoordigt een enkel bestand binnen tar-archief.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extraheert het item naar de opgegeven stream. |
| [extract(String path)](#extract-java.lang.String-) | Extraheert het item naar het bestandssysteem via het opgegeven pad. |
| [getLength()](#getLength--) | Haalt de lengte van het item op in bytes. |
| [getModificationTime()](#getModificationTime--) | Haalt de wijzigingstijd van het bestand of de map op. |
| [getName()](#getName--) | Haalt de naam van het item binnen het archief op. |
| [getUncompressedSize()](#getUncompressedSize--) | Haalt de grootte van een origineel bestand op. |
| [isDirectory()](#isDirectory--) | Haalt een waarde op die aangeeft of het item een map vertegenwoordigt. |
| [open()](#open--) | Opent het item voor extractie en levert een stream met de inhoud van het item. |
| [setName(String value)](#setName-java.lang.String-) | Stelt de naam van het item binnen het archief in. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extraheert het item naar de opgegeven stream.

Extraheer een item van het tar-archief.

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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | het pad naar het bestemmingsbestand. Als het bestand al bestaat, wordt het overschreven |

**Returns:**
java.io.File - de bestandsinformatie van het geëxtraheerde bestand
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


Haalt de wijzigingstijd van het bestand of de map op.

**Returns:**
java.util.Date - de wijzigingstijd van het bestand of de map.
### getName() {#getName--}
```
public final String getName()
```


Haalt de naam van het item binnen het archief op.

**Returns:**
java.lang.String - de naam van het item binnen het archief
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Haalt de grootte van een origineel bestand op.

Heeft dezelfde waarde als `Length`([getLength](../../com.aspose.zip/tarentry\#getLength--))

**Returns:**
long - de grootte van een origineel bestand.
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Haalt een waarde op die aangeeft of het item een map vertegenwoordigt.

**Returns:**
boolean - een waarde die aangeeft of de entry een map vertegenwoordigt
### open() {#open--}
```
public final InputStream open()
```


Opent het item voor extractie en levert een stream met de inhoud van het item.


Gebruik:

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

