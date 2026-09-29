---
title: "IsoEntry"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Stellt einen Datei- oder Verzeichnis-Eintrag innerhalb eines ISO-Archivs dar."
type: docs
weight: 72
url: /de/java/com.aspose.zip/isoentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class IsoEntry implements IArchiveFileEntry
```

Stellt einen Eintrag (Datei oder Verzeichnis) innerhalb eines ISO-Archivs dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrahiert den Eintrag in den bereitgestellten Stream. |
| [extract(String path)](#extract-java.lang.String-) | Extrahiert den Eintrag in das Dateisystem über den angegebenen Pfad. |
| [getLength()](#getLength--) | Ermittelt die Länge des Eintrags. |
| [getModificationTime()](#getModificationTime--) | Ermittelt das Datum und die Uhrzeit der letzten Änderung. |
| [getName()](#getName--) | Ermittelt den Namen des Eintrags. |
| [isDirectory()](#isDirectory--) | Ermittelt einen Wert, der angibt, ob der Eintrag ein Verzeichnis ist. |
| [toString()](#toString--) | Gibt eine Zeichenkette zurück, die den aktuellen Eintrag darstellt. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public void extract(OutputStream destination)
```


Extrahiert den Eintrag in den bereitgestellten Stream.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Ziel | java.io.OutputStream | Ziel-Stream |

### extract(String path) {#extract-java.lang.String-}
```
public File extract(String path)
```


Extrahiert den Eintrag in das Dateisystem über den angegebenen Pfad.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | java.lang.String | Der Pfad zur Zieldatei. Wenn die Datei bereits existiert, wird sie überschrieben. |

**Returns:**
java.io.File - java.io.File-Instanz, die extrahierte Daten enthält
### getLength() {#getLength--}
```
public Long getLength()
```


Ermittelt die Länge des Eintrags.

**Returns:**
java.lang.Long - die Länge des Eintrags
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Ermittelt das Datum und die Uhrzeit der letzten Änderung.

**Returns:**
java.util.Date - Datum und Uhrzeit der letzten Änderung
### getName() {#getName--}
```
public final String getName()
```


Ermittelt den Namen des Eintrags.

**Returns:**
java.lang.String - der Name des Eintrags
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Ermittelt einen Wert, der angibt, ob der Eintrag ein Verzeichnis ist.

**Returns:**
boolean - ein Wert, der angibt, ob der Eintrag ein Verzeichnis darstellt
### toString() {#toString--}
```
public String toString()
```


Gibt eine Zeichenkette zurück, die den aktuellen Eintrag darstellt.

**Returns:**
java.lang.String - der Name des Eintrags
