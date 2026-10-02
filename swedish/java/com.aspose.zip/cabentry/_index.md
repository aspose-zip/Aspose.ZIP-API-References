---
title: "CabEntry"
second_title: "Aspose.ZIP för Java API-referens"
description: "Representerar en enskild fil i ett cab-arkiv."
type: docs
weight: 46
url: /sv/java/com.aspose.zip/cabentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public final class CabEntry implements IArchiveFileEntry
```

Representerar en enskild fil i ett cab-arkiv.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extraherar posten till den angivna strömmen. |
| [extract(String path)](#extract-java.lang.String-) | Extraherar posten till filsystemet enligt den angivna sökvägen. |
| [getLength()](#getLength--) | Hämtar längden på posten i byte. |
| [getModificationTime()](#getModificationTime--) | Hämtar senaste ändringsdatum och -tid. |
| [getName()](#getName--) | Hämtar namnet på posten i arkivet. |
| [open()](#open--) | Öppnar posten för extrahering och tillhandahåller en ström med postens innehåll. |
| [toString()](#toString--) | Returnerar en strängrepresentation av instansen av klassen [CabEntry](../../com.aspose.zip/cabentry). |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extraherar posten till den angivna strömmen.

Extrahera en post från ett CAB-arkiv.

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| path | java.lang.String | sökvägen till destinationsfilen. Om filen redan finns kommer den att skrivas över. |

**Returns:**
java.io.File - filinformationen för en sammansatt fil
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


Hämtar senaste ändringsdatum och -tid.

**Returns:**
java.util.Date - senaste ändringsdatum och tid.
### getName() {#getName--}
```
public final String getName()
```


Hämtar namnet på posten i arkivet.

**Returns:**
java.lang.String – namnet på posten i arkivet
### open() {#open--}
```
public final InputStream open()
```


Öppnar posten för extrahering och tillhandahåller en ström med postens innehåll.

Användning:

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
