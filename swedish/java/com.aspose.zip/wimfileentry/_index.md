---
title: "WimFileEntry"
second_title: "Aspose.ZIP för Java API-referens"
description: "Representerar en enskild fil i wim-arkivet."
type: docs
weight: 133
url: /sv/java/com.aspose.zip/wimfileentry/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.WimEntry](../../com.aspose.zip/wimentry)

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public final class WimFileEntry extends WimEntry implements IArchiveFileEntry
```

Representerar en enskild fil i wim-arkivet.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extraherar posten till den angivna strömmen. |
| [extract(String path)](#extract-java.lang.String-) | Extraherar posten till filsystemet enligt den angivna sökvägen. |
| [getLength()](#getLength--) | Hämtar längden på posten i byte. |
| [open()](#open--) | Öppnar posten för extrahering och tillhandahåller en ström med postens innehåll. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extraherar posten till den angivna strömmen.

Extrahera en post från wim‑arkivet.

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| path | java.lang.String | sökvägen till destinationsfilen. Om filen redan finns kommer den att skrivas över. |

**Returns:**
java.io.File - filinformationen för den extraherade filen
### getLength() {#getLength--}
```
public final Long getLength()
```


Hämtar längden på posten i byte.

**Returns:**
java.lang.Long - längden på posten i byte
### open() {#open--}
```
public final InputStream open()
```


Öppnar posten för extrahering och tillhandahåller en ström med postens innehåll.

Användning:

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
