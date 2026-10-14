---
title: "WimEntry"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Stellt eine einzelne Datei oder ein Verzeichnis innerhalb eines Wim-Images dar."
type: docs
weight: 132
url: /de/java/com.aspose.zip/wimentry/
---

**Inheritance:**
java.lang.Object
```
public abstract class WimEntry
```

Stellt eine einzelne Datei oder ein Verzeichnis innerhalb eines Wim-Images dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getAlternateDataStreams()](#getAlternateDataStreams--) | Liefert die Namen der alternativen Datenströme für die Datei oder das Verzeichnis. |
| [getArchive()](#getArchive--) | Gibt das Archiv zurück, zu dem der Eintrag gehört. |
| [getChangeTime()](#getChangeTime--) | Liefert den letzten Zeitpunkt, zu dem die Datei oder das Verzeichnis geändert wurde. |
| [getCreationTime()](#getCreationTime--) | Liefert den Erstellungszeitpunkt der Datei oder des Verzeichnisses. |
| [getFileAttributes()](#getFileAttributes--) | Liefert die Attribute der Datei oder des Verzeichnisses. |
| [getFullPath()](#getFullPath--) | Liefert den vollständigen Pfad des Eintrags innerhalb des Images. |
| [getHardLink()](#getHardLink--) | Liefert die Hardlink-ID der Datei oder des Verzeichnisses. |
| [getImage()](#getImage--) | Liefert das Image, zu dem der Eintrag gehört. |
| [getLastAccessTime()](#getLastAccessTime--) | Liefert den letzten Zugriffszeitpunkt der Datei oder des Verzeichnisses. |
| [getLastWriteTime()](#getLastWriteTime--) | Liefert den Änderungszeitpunkt der Datei oder des Verzeichnisses. |
| [getModificationTime()](#getModificationTime--) | Liefert den Änderungszeitpunkt der Datei oder des Verzeichnisses. |
| [getName()](#getName--) | Liefert den Namen des Eintrags innerhalb des Images. |
| [getParent()](#getParent--) | Liefert das übergeordnete Verzeichnis, zu dem der Eintrag gehört. |
| [getShortName()](#getShortName--) | Liefert den Kurznamen des Eintrags innerhalb des Images. |
| [hasHardLinks()](#hasHardLinks--) | Liefert, ob die Datei oder das Verzeichnis unter anderen Namen bekannt ist. |
| [isDirectory()](#isDirectory--) | Liefert einen Wert, der angibt, ob der Eintrag ein Verzeichnis darstellt. |
| [toString()](#toString--) | Gibt die Zeichenkettenrepräsentation der Instanz der Klasse [WimEntry](../../com.aspose.zip/wimentry) zurück. |
### getAlternateDataStreams() {#getAlternateDataStreams--}
```
public final String[] getAlternateDataStreams()
```


Liefert die Namen der alternativen Datenströme für die Datei oder das Verzeichnis.

**Returns:**
java.lang.String[] - die Namen der alternativen Datenströme für die Datei oder das Verzeichnis
### getArchive() {#getArchive--}
```
public final WimArchive getArchive()
```


Gibt das Archiv zurück, zu dem der Eintrag gehört.

**Returns:**
[WimArchive](../../com.aspose.zip/wimarchive) - the archive the entry belongs to
### getChangeTime() {#getChangeTime--}
```
public final Date getChangeTime()
```


Liefert den letzten Zeitpunkt, zu dem die Datei oder das Verzeichnis geändert wurde.

**Returns:**
java.util.Date - die letzte Zeit, zu der die Datei oder das Verzeichnis geändert wurde
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


Liefert den Erstellungszeitpunkt der Datei oder des Verzeichnisses.

**Returns:**
java.util.Date - die Erstellungszeit der Datei oder des Verzeichnisses
### getFileAttributes() {#getFileAttributes--}
```
public final int getFileAttributes()
```


Liefert die Attribute der Datei oder des Verzeichnisses.

**Returns:**
int - die Attribute der Datei oder des Verzeichnisses
### getFullPath() {#getFullPath--}
```
public final String getFullPath()
```


Liefert den vollständigen Pfad des Eintrags innerhalb des Images.

**Returns:**
java.lang.String - der vollständige Pfad des Eintrags im Image
### getHardLink() {#getHardLink--}
```
public final long getHardLink()
```


Liefert die Hardlink-ID der Datei oder des Verzeichnisses.

**Returns:**
long - die Hardlink-ID der Datei oder des Verzeichnisses
### getImage() {#getImage--}
```
public final WimImage getImage()
```


Liefert das Image, zu dem der Eintrag gehört.

**Returns:**
[WimImage](../../com.aspose.zip/wimimage) - the image the entry belongs to
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


Liefert den Namen des Eintrags innerhalb des Images.

**Returns:**
java.lang.String - der Name des Eintrags im Image
### getParent() {#getParent--}
```
public final WimDirectoryEntry getParent()
```


Liefert das übergeordnete Verzeichnis, zu dem der Eintrag gehört.

**Returns:**
[WimDirectoryEntry](../../com.aspose.zip/wimdirectoryentry) - the parent directory the entry belongs to
### getShortName() {#getShortName--}
```
public final String getShortName()
```


Liefert den Kurznamen des Eintrags innerhalb des Images.

**Returns:**
java.lang.String - der Kurzname des Eintrags im Image
### hasHardLinks() {#hasHardLinks--}
```
public final boolean hasHardLinks()
```


Liefert, ob die Datei oder das Verzeichnis unter anderen Namen bekannt ist.

**Returns:**
boolean - ob die Datei oder das Verzeichnis unter anderen Namen bekannt ist
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


Gibt die Zeichenkettenrepräsentation der Instanz der Klasse [WimEntry](../../com.aspose.zip/wimentry) zurück.

**Returns:**
java.lang.String - Zeichenkettenrepräsentation dieses Objekts
