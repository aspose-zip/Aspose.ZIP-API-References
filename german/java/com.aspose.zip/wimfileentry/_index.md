---
title: "WimFileEntry"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Stellt eine einzelne Datei innerhalb eines Wim-Archivs dar."
type: docs
weight: 133
url: /de/java/com.aspose.zip/wimfileentry/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.WimEntry](../../com.aspose.zip/wimentry)

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public final class WimFileEntry extends WimEntry implements IArchiveFileEntry
```

Stellt eine einzelne Datei innerhalb eines Wim-Archivs dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrahiert den Eintrag in den bereitgestellten Stream. |
| [extract(String path)](#extract-java.lang.String-) | Extrahiert den Eintrag in das Dateisystem über den angegebenen Pfad. |
| [getLength()](#getLength--) | Gibt die Länge des Eintrags in Bytes zurück. |
| [open()](#open--) | Öffnet den Eintrag zum Extrahieren und stellt einen Stream mit dem Eintragsinhalt bereit. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extrahiert den Eintrag in den bereitgestellten Stream.

Extrahieren Sie einen Eintrag aus einem wim-Archiv.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | java.lang.String | Der Pfad zur Zieldatei. Wenn die Datei bereits existiert, wird sie überschrieben. |

**Returns:**
java.io.File - die Dateiinformation der extrahierten Datei
### getLength() {#getLength--}
```
public final Long getLength()
```


Gibt die Länge des Eintrags in Bytes zurück.

**Returns:**
java.lang.Long – die Länge des Eintrags in Bytes
### open() {#open--}
```
public final InputStream open()
```


Öffnet den Eintrag zum Extrahieren und stellt einen Stream mit dem Eintragsinhalt bereit.

Verwendung:

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
