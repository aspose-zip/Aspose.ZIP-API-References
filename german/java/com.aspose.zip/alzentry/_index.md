---
title: "AlzEntry"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Stellt einen Dateieintrag in einem ALZ-Archiv zusammen mit seinen Metadaten dar."
type: docs
weight: 13
url: /de/java/com.aspose.zip/alzentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class AlzEntry implements IArchiveFileEntry
```

Stellt einen Dateieintrag in einem ALZ-Archiv zusammen mit seinen Metadaten dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrahiert den Eintrag in einen beschreibbaren Stream. |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | Extrahiert den Eintrag in einen beschreibbaren Stream unter Verwendung eines optionalen Passworts. |
| [extract(String path)](#extract-java.lang.String-) | Extrahiert den Eintrag in die angegebene Datei. |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | Extrahiert den Eintrag in die angegebene Datei unter Verwendung eines optionalen Passworts. |
| [getCompressedSize()](#getCompressedSize--) | Ermittelt die komprimierte Größe der Eintragsdaten in Bytes. |
| [getLength()](#getLength--) | Ermittelt die dekomprimierte Länge dieses Eintrags. |
| [getName()](#getName--) | Ermittelt den im Archiv gespeicherten Eintragsnamen. |
| [getUncompressedSize()](#getUncompressedSize--) | Ermittelt die dekomprimierte Größe der Eintragsdaten in Bytes. |
| [isDirectory()](#isDirectory--) | Ermittelt, ob dieser Eintrag ein Verzeichnis darstellt. |
| [open()](#open--) | Öffnet den Eintrag und stellt einen Stream mit dekomprimierten Daten bereit. |
| [open(String password)](#open-java.lang.String-) | Öffnet den Eintrag und stellt einen Stream mit dekomprimierten Daten bereit. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extrahiert den Eintrag in einen beschreibbaren Stream.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Ziel | java.io.OutputStream | Ziel-Stream |

### extract(OutputStream destination, String password) {#extract-java.io.OutputStream-java.lang.String-}
```
public final void extract(OutputStream destination, String password)
```


Extrahiert den Eintrag in einen beschreibbaren Stream unter Verwendung eines optionalen Passworts.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Ziel | java.io.OutputStream | Ziel-Stream |
| password | java.lang.String | Optionales Passwort für diesen Eintrag |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extrahiert den Eintrag in die angegebene Datei. Eine vorhandene Datei wird überschrieben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | java.lang.String | Ziel-Dateipfad |

**Returns:**
java.io.File - extrahierte Datei
### extract(String path, String password) {#extract-java.lang.String-java.lang.String-}
```
public final File extract(String path, String password)
```


Extrahiert den Eintrag in die angegebene Datei unter Verwendung eines optionalen Passworts.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | java.lang.String | Ziel-Dateipfad |
| password | java.lang.String | Optionales Passwort für diesen Eintrag |

**Returns:**
java.io.File - extrahierte Datei
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Ermittelt die komprimierte Größe der Eintragsdaten in Bytes.

**Returns:**
long - komprimierte Größe in Bytes
### getLength() {#getLength--}
```
public final Long getLength()
```


Ermittelt die dekomprimierte Länge dieses Eintrags.

**Returns:**
java.lang.Long - unkomprimierte Länge in Bytes
### getName() {#getName--}
```
public final String getName()
```


Ermittelt den im Archiv gespeicherten Eintragsnamen.

**Returns:**
java.lang.String - Eintragsname
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Ermittelt die dekomprimierte Größe der Eintragsdaten in Bytes.

**Returns:**
long - unkomprimierte Größe in Bytes
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Ermittelt, ob dieser Eintrag ein Verzeichnis darstellt.

**Returns:**
boolean - `true` für einen Verzeichniseintrag
### open() {#open--}
```
public final InputStream open()
```


Öffnet den Eintrag und stellt einen Stream mit dekomprimierten Daten bereit.

**Returns:**
java.io.InputStream - Stream, der dekomprimierte Eintragsdaten enthält
### open(String password) {#open-java.lang.String-}
```
public final InputStream open(String password)
```


Öffnet den Eintrag und stellt einen Stream mit dekomprimierten Daten bereit.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| password | java.lang.String | Optionales Passwort für diesen Eintrag |

**Returns:**
java.io.InputStream - Stream, der dekomprimierte Eintragsdaten enthält
