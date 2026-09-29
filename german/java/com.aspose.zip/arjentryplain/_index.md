---
title: "ArjEntryPlain"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Stellt eine einzelne Datei innerhalb eines ARJ-Archivs dar."
type: docs
weight: 38
url: /de/java/com.aspose.zip/arjentryplain/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class ArjEntryPlain implements IArchiveFileEntry
```

Stellt eine einzelne Datei innerhalb eines ARJ-Archivs dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [extract(File file)](#extract-java.io.File-) | Extrahiert einen ARJ‑Archiv‑Eintrag in eine Datei. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrahiert den Eintrag in den bereitgestellten Stream. |
| [extract(String path)](#extract-java.lang.String-) | Extrahiert den Eintrag in das Dateisystem über den angegebenen Pfad. |
| [getCompressedSize()](#getCompressedSize--) | Liefert die Größe der komprimierten Datei. |
| [getLength()](#getLength--) | Gibt die Länge des Eintrags in Bytes zurück. |
| [getName()](#getName--) | Liefert den Namen des Eintrags im Archiv. |
| [getUncompressedSize()](#getUncompressedSize--) | Liefert die Größe der Originaldatei. |
### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Extrahiert einen ARJ‑Archiv‑Eintrag in eine Datei.

```

``````

try (FileInputStream arjFile = new FileInputStream("sourceFileName")) {
try (ArjArchive archive = new ArjArchive(arjFile)) {
archive.getEntries().get(0).extract(new File(\"extracted.bin\"));
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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | java.lang.String | Der Pfad zur Zieldatei. Wenn die Datei bereits existiert, wird sie überschrieben. |

**Returns:**
java.io.File - die Dateiinformationen der zusammengesetzten Datei
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Liefert die Größe der komprimierten Datei.

**Returns:**
long – die Größe der komprimierten Datei
### getLength() {#getLength--}
```
public final Long getLength()
```


Gibt die Länge des Eintrags in Bytes zurück.

**Returns:**
java.lang.Long – die Länge des Eintrags in Bytes
### getName() {#getName--}
```
public final String getName()
```


Liefert den Namen des Eintrags im Archiv.

**Returns:**
java.lang.String - Name des Eintrags im Archiv
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Liefert die Größe der Originaldatei.

**Returns:**
long - Größe der Originaldatei
