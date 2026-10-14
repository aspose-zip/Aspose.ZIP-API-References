---
title: "XarEntry"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Stellt einen einzelnen Eintrag innerhalb eines XAR-Archivs dar."
type: docs
weight: 140
url: /de/java/com.aspose.zip/xarentry/
---

**Inheritance:**
java.lang.Object
```
public abstract class XarEntry
```

Stellt einen einzelnen Eintrag innerhalb eines XAR-Archivs dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getCreationTime()](#getCreationTime--) | Liefert den Erstellungszeitpunkt der Datei oder des Verzeichnisses. |
| [getFullPath()](#getFullPath--) | Liefert den vollständigen Pfad des Eintrags im Archiv. |
| [getLastAccessTime()](#getLastAccessTime--) | Liefert den letzten Zugriffszeitpunkt der Datei oder des Verzeichnisses. |
| [getLastWriteTime()](#getLastWriteTime--) | Liefert den Änderungszeitpunkt der Datei oder des Verzeichnisses. |
| [getModificationTime()](#getModificationTime--) | Liefert den Änderungszeitpunkt der Datei oder des Verzeichnisses. |
| [getName()](#getName--) | Gibt den Namen des Eintrags im Archiv zurück. |
| [getParent()](#getParent--) | Liefert das übergeordnete Verzeichnis, zu dem der Eintrag gehört. |
| [isDirectory()](#isDirectory--) | Liefert einen Wert, der angibt, ob der Eintrag ein Verzeichnis darstellt. |
| [toString()](#toString--) | Gibt die Zeichenkettenrepräsentation der Instanz der Klasse [XarEntry](../../com.aspose.zip/xarentry) zurück. |
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


Liefert den Erstellungszeitpunkt der Datei oder des Verzeichnisses.

**Returns:**
java.util.Date - die Erstellungszeit der Datei oder des Verzeichnisses
### getFullPath() {#getFullPath--}
```
public final String getFullPath()
```


Liefert den vollständigen Pfad des Eintrags im Archiv.

**Returns:**
java.lang.String - der vollständige Pfad des Eintrags im Archiv
### getLastAccessTime() {#getLastAccessTime--}
```
public final Date getLastAccessTime()
```


Liefert den letzten Zugriffszeitpunkt der Datei oder des Verzeichnisses.

**Returns:**
java.util.Date - die letzte Zugriffszeit der Datei oder des Verzeichnisses
### getLastWriteTime() {#getLastWriteTime--}
```
public final Date getLastWriteTime()
```


Liefert den Änderungszeitpunkt der Datei oder des Verzeichnisses.

**Returns:**
java.util.Date - die Änderungszeit der Datei oder des Verzeichnisses
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Liefert den Änderungszeitpunkt der Datei oder des Verzeichnisses.

**Returns:**
java.util.Date - die Änderungszeit der Datei oder des Verzeichnisses
### getName() {#getName--}
```
public final String getName()
```


Gibt den Namen des Eintrags im Archiv zurück.

**Returns:**
java.lang.String - der Name des Eintrags im Archiv
### getParent() {#getParent--}
```
public final XarDirectoryEntry getParent()
```


Liefert das übergeordnete Verzeichnis, zu dem der Eintrag gehört.

**Returns:**
[XarDirectoryEntry](../../com.aspose.zip/xardirectoryentry) - the parent directory the entry belongs to
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Liefert einen Wert, der angibt, ob der Eintrag ein Verzeichnis darstellt.

**Returns:**
boolean - ein Wert, der angibt, ob der Eintrag ein Verzeichnis darstellt
### toString() {#toString--}
```
public String toString()
```


Gibt die Zeichenkettenrepräsentation der Instanz der Klasse [XarEntry](../../com.aspose.zip/xarentry) zurück.

**Returns:**
java.lang.String - Zeichenkettenrepräsentation dieses Objekts
