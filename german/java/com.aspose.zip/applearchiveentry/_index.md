---
title: "AppleArchiveEntry"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Stellt einen Datei- oder Verzeichniseintrag innerhalb eines . dar."
type: docs
weight: 17
url: /de/java/com.aspose.zip/applearchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public final class AppleArchiveEntry implements IArchiveFileEntry
```

Stellt einen Datei- oder Verzeichniseintrag innerhalb eines [AppleArchive](../../com.aspose.zip/applearchive) dar.

Eine Instanz dieser Klasse kann entweder einen Eintrag darstellen, der aus einem bestehenden Apple-Archiv geparst wurde, oder einen Eintrag, der zu einem gerade erstellten Archiv hinzugefügt wird.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrahiert den Eintrag in den bereitgestellten Stream. |
| [extract(String path)](#extract-java.lang.String-) | Extrahiert einen Apple-Archiv-Eintrag anhand des Pfads in ein Dateisystem. |
| [getLength()](#getLength--) | Ermittelt die unkomprimierte Länge des Eintrags in Bytes. |
| [getName()](#getName--) | Ermittelt den Pfad des Eintrags innerhalb des Archivs. |
| [isDirectory()](#isDirectory--) | Liefert einen Wert, der angibt, ob der Eintrag ein Verzeichnis darstellt. |
| [open()](#open--) | Öffnet den Eintrag zum Extrahieren und liefert einen Stream mit dem Eintragsinhalt. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public void extract(OutputStream destination)
```


Extrahiert den Eintrag in den bereitgestellten Stream.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Ziel | java.io.OutputStream | Ziel-Stream. Muss beschreibbar sein. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extrahiert einen Apple-Archiv-Eintrag anhand des Pfads in ein Dateisystem.

```

``````

try (FileInputStream aaFile = new FileInputStream(\"archive.aa\")) {
try (AppleArchive archive = new AppleArchive(aaFile)) {
archive.getEntries().get(0).extract(\"extracted.bin\");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | Path to file which will store decompressed data. |

**Returns:**
java.io.File - FileSystemInfoInstance containing extracted data.
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets the uncompressed length of the entry in bytes.

For directory entries the value is zero. For entries created from a non-seekable source stream the length can be unknown.

**Returns:**
java.lang.Long - the uncompressed length of the entry in bytes.
### getName() {#getName--}
```
public final String getName()
```


Gets the path of the entry inside the archive.

The value is the archive path recorded for the entry. Directory entries usually end with Forward slash (`/`).

**Returns:**
java.lang.String - the path of the entry inside the archive.
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Gets a value indicating whether the entry represents a directory.

**Returns:**
boolean - a value indicating whether the entry represents a directory.
### open() {#open--}
```
public final InputStream open()
```


Opens the entry for extraction and provides a stream with the entry content.

**Returns:**
java.io.InputStream - A readable stream that contains the extracted entry data.
