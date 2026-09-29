---
title: "LhaArchiveEntry"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Stellt eine einzelne Datei innerhalb eines Lha-Archivs dar."
type: docs
weight: 76
url: /de/java/com.aspose.zip/lhaarchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class LhaArchiveEntry implements IArchiveFileEntry
```

Stellt eine einzelne Datei innerhalb eines Lha-Archivs dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [extract(File file)](#extract-java.io.File-) | Extrahiert Lha-Archiveintrag in eine Datei. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrahiert den Eintrag in den bereitgestellten Stream. |
| [extract(String path)](#extract-java.lang.String-) | Extrahiert Lha-Archiveintrag in ein Dateisystem anhand des Pfads. |
| [getLastModified()](#getLastModified--) | Ermittelt die zuletzt geänderte Zeit des Eintrags. |
| [getLength()](#getLength--) | Gibt die Länge des Eintrags in Bytes zurück. |
| [getModificationTime()](#getModificationTime--) | Ermittelt die zuletzt geänderte Zeit des Eintrags. |
| [getName()](#getName--) | Ermittelt den Namen des Eintrags. |
| [getPath()](#getPath--) | Ermittelt den vollständigen Pfad zum Eintrag. |
| [isDirectory()](#isDirectory--) | Ermittelt einen Wert, der angibt, ob dieser Eintrag ein Verzeichnis ist. |
### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Extrahiert Lha-Archiveintrag in eine Datei.

```

``````

try (FileInputStream lhaFile = new FileInputStream(\"archive.lha\")) {
try (LhaArchive archive = new LhaArchive(lhaFile)) {
archive.getEntries().get(0).extract(new File(\"extracted.bin\"));
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | File for storing decompressed data.

Does nothing for directory entry |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts the entry to the stream provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts Lha archive entry to a filesystem by path.

```

``````

     try (FileInputStream lhaFile = new FileInputStream("archive.lha")) {
         try (LhaArchive archive = new LhaArchive(lhaFile)) {
             archive.getEntries().get(0).extract("extracted.bin");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | java.lang.String | Der Pfad zu der Datei, die die dekomprimierten Daten speichert. |

**Returns:**
java.io.File - java.io.File-Instanz, die extrahierte Daten enthält
### getLastModified() {#getLastModified--}
```
public final Date getLastModified()
```


Ermittelt die zuletzt geänderte Zeit des Eintrags.

**Returns:**
java.util.Date – die zuletzt geänderte Zeit des Eintrags.
### getLength() {#getLength--}
```
public final Long getLength()
```


Gibt die Länge des Eintrags in Bytes zurück.

**Returns:**
java.lang.Long – die Länge des Eintrags in Bytes
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Ermittelt die zuletzt geänderte Zeit des Eintrags.

**Returns:**
java.util.Date – die zuletzt geänderte Zeit des Eintrags.
### getName() {#getName--}
```
public final String getName()
```


Ermittelt den Namen des Eintrags.

Archive nur zur Kompression, wie gzip, bzip2, lzip, lzma, xz, z, haben den Namen \"File.bin\", sofern kein anderer Name in den Headern gefunden wird.

**Returns:**
java.lang.String - der Name des Eintrags
### getPath() {#getPath--}
```
public final String getPath()
```


Ermittelt den vollständigen Pfad zum Eintrag.

**Returns:**
java.lang.String – der vollständige Pfad zum Eintrag.
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Ermittelt einen Wert, der angibt, ob dieser Eintrag ein Verzeichnis ist.

**Returns:**
boolean – ein Wert, der angibt, ob dieser Eintrag ein Verzeichnis ist.
