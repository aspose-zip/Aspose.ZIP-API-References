---
title: "WimFileEntry"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Vertegenwoordigt een enkel bestand binnen wim-archief."
type: docs
weight: 133
url: /nl/java/com.aspose.zip/wimfileentry/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.WimEntry](../../com.aspose.zip/wimentry)

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public final class WimFileEntry extends WimEntry implements IArchiveFileEntry
```

Vertegenwoordigt een enkel bestand binnen wim-archief.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extraheert het item naar de opgegeven stream. |
| [extract(String path)](#extract-java.lang.String-) | Extraheert het item naar het bestandssysteem via het opgegeven pad. |
| [getLength()](#getLength--) | Haalt de lengte van het item op in bytes. |
| [open()](#open--) | Opent het item voor extractie en levert een stream met de inhoud van het item. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extraheert het item naar de opgegeven stream.

Extraheer een item van een wim-archief.

```

``````

try (WimArchive archive = new WimArchive("archive.wim")) {
archive.getImages().get_Item(0).getRootDirectory().getFiles().get(0).extract(httpResponseStream);
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

     try (WimArchive archive = new WimArchive("archive.wim")) {
         archive.getImages().get_Item(0).getRootDirectory().getFiles().get(0).extract("data.bin");
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
### open() {#open--}
```
public final InputStream open()
```


Opent het item voor extractie en levert een stream met de inhoud van het item.

Gebruik:

```

``````

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
