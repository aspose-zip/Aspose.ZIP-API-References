---
title: "LzxArchiveEntry"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Stellt eine einzelne Datei innerhalb eines LZX-Archivs dar."
type: docs
weight: 90
url: /de/java/com.aspose.zip/lzxarchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class LzxArchiveEntry implements IArchiveFileEntry
```

Stellt eine einzelne Datei innerhalb eines LZX-Archivs dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrahiert den Eintrag in den bereitgestellten Stream. |
| [extract(String path)](#extract-java.lang.String-) | Extrahiert Lzx-Archiveintrag in ein Dateisystem anhand des Pfads. |
| [getCommentary()](#getCommentary--) | Liefert den Kommentar. |
| [getCompressedSize()](#getCompressedSize--) | Ermittelt die Größe der komprimierten Datei. |
| [getLength()](#getLength--) | Gibt die Länge des Eintrags in Bytes zurück. |
| [getModificationTime()](#getModificationTime--) | Ermittelt die zuletzt geänderte Zeit des Eintrags. |
| [getName()](#getName--) | Ermittelt den Namen des Eintrags. |
| [getUncompressedSize()](#getUncompressedSize--) | Liefert die Größe der Originaldatei. |
| [isDirectory()](#isDirectory--) | Ermittelt einen Wert, der angibt, ob dieser Eintrag ein Verzeichnis ist. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
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


Extrahiert Lzx-Archiveintrag in ein Dateisystem anhand des Pfads.

```

``````

try (FileInputStream lzxFile = new FileInputStream("archive.lzx")) {
try (LzxArchive archive = new LzxArchive(lzxFile)) {
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
### getCommentary() {#getCommentary--}
```
public final String getCommentary()
```


Gets the commentary.

**Returns:**
java.lang.String - the commentary.
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Gets size of the compressed file.

**Returns:**
long - size of the compressed file.
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets the length of the entry in bytes.

**Returns:**
java.lang.Long - the length of the entry in bytes
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Gets the last modified time of the entry.

**Returns:**
java.util.Date - the last modified time of the entry.
### getName() {#getName--}
```
public final String getName()
```


Gets the name of the entry.

Archives for compression only, such as gzip, bzip2, lzip, lzma, xz, z has name "File.bin" unless another name can be found in headers.

**Returns:**
java.lang.String - the name of the entry
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets size of the original file.

**Returns:**
long - size of the original file.
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Gets a value indicating whether this entry is a directory.

**Returns:**
boolean - a value indicating whether this entry is a directory.
