---
title: "SplitArchiveSaveOptions"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Optionen zum Speichern eines mehrteiligen ZIP-Archivs."
type: docs
weight: 122
url: /de/java/com.aspose.zip/splitarchivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class SplitArchiveSaveOptions
```

Optionen zum Speichern eines mehrteiligen ZIP-Archivs.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [SplitArchiveSaveOptions(String fileName, long segmentSize)](#SplitArchiveSaveOptions-java.lang.String-long-) | Instanziiert Einstellungen zum Speichern eines mehrteiligen ZIP-Archivs. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getArchiveComment()](#getArchiveComment--) | Liefert optionalen Kommentar für die Zip-Datei. |
| [getCloseEntrySource()](#getCloseEntrySource--) | Liefert einen Wert, der angibt, ob die Quellen der Einträge unmittelbar nach dem Komprimieren eines Eintrags geschlossen werden sollen. |
| [getEncoding()](#getEncoding--) | Liefert die Kodierung zum Konvertieren von Dateinamen und anderen Zeichenketten in Bytes. |
| [getEventsBag()](#getEventsBag--) | Liefert den Container von Ereignissen, die beim Speichern des Archivs ausgelöst werden. |
| [getFileName()](#getFileName--) | Liefert den Namen der Segmente ohne Erweiterung. |
| [getSegmentSize()](#getSegmentSize--) | Liefert die Größe des Segments. |
| [setArchiveComment(String value)](#setArchiveComment-java.lang.String-) | Setzt optionalen Kommentar für die Zip-Datei. |
| [setCloseEntrySource(boolean value)](#setCloseEntrySource-boolean-) | Setzt einen Wert, der angibt, ob die Quellen der Einträge unmittelbar nach dem Komprimieren eines Eintrags geschlossen werden sollen. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Setzt die Kodierung zum Konvertieren von Dateinamen und anderen Zeichenketten in Bytes. |
| [setEventsBag(EventsBag value)](#setEventsBag-com.aspose.zip.EventsBag-) | Setzt den Container von Ereignissen, die beim Speichern des Archivs ausgelöst werden. |
### SplitArchiveSaveOptions(String fileName, long segmentSize) {#SplitArchiveSaveOptions-java.lang.String-long-}
```
public SplitArchiveSaveOptions(String fileName, long segmentSize)
```


Instanziiert Einstellungen zum Speichern eines mehrteiligen ZIP-Archivs.

Einige Volumen können kleiner als `segmentSize` sein. In den meisten Fällen ist das letzte Segment kleiner, aber selten können reguläre Segmente ebenfalls zu klein sein.

Dateinamen werden wie folgt sein: `fileName`.z01, `fileName`.z02, ..., `fileName`.z(n-1), `fileName`.zip.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | java.lang.String | Name für Volumen. Kann mit oder ohne .zip-Erweiterung sein. |
| segmentSize | long | Größe des Volumens. |

### getArchiveComment() {#getArchiveComment--}
```
public final String getArchiveComment()
```


Liefert optionalen Kommentar für die Zip-Datei.

**Returns:**
java.lang.String - optionaler Kommentar für die Zip-Datei.
### getCloseEntrySource() {#getCloseEntrySource--}
```
public final boolean getCloseEntrySource()
```


Liefert einen Wert, der angibt, ob die Quellen der Einträge unmittelbar nach dem Komprimieren eines Eintrags geschlossen werden sollen.

**Returns:**
boolean - ein Wert, der angibt, ob die Quellen der Einträge unmittelbar nach der Komprimierung eines Eintrags geschlossen werden sollen.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Liefert die Kodierung zum Konvertieren von Dateinamen und anderen Zeichenketten in Bytes.

Falls nicht gesetzt, wird Codepage 437 verwendet.

**Returns:**
java.nio.charset.Charset - Kodierung zum Konvertieren von Dateinamen und anderen Zeichenketten in Bytes.
### getEventsBag() {#getEventsBag--}
```
public final EventsBag getEventsBag()
```


Liefert den Container von Ereignissen, die beim Speichern des Archivs ausgelöst werden.

**Returns:**
[EventsBag](../../com.aspose.zip/eventsbag) - container of events raising on archive saving.
### getFileName() {#getFileName--}
```
public final String getFileName()
```


Liefert den Namen der Segmente ohne Erweiterung.

**Returns:**
java.lang.String - der Name der Segmente ohne Erweiterung.
### getSegmentSize() {#getSegmentSize--}
```
public final long getSegmentSize()
```


Liefert die Größe des Segments.

**Returns:**
long - die Größe des Segments.
### setArchiveComment(String value) {#setArchiveComment-java.lang.String-}
```
public final void setArchiveComment(String value)
```


Setzt optionalen Kommentar für die Zip-Datei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | optionaler Kommentar für die Zip-Datei. |

### setCloseEntrySource(boolean value) {#setCloseEntrySource-boolean-}
```
public final void setCloseEntrySource(boolean value)
```


Setzt einen Wert, der angibt, ob die Quellen der Einträge unmittelbar nach dem Komprimieren eines Eintrags geschlossen werden sollen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | Ein Wert, der angibt, ob die Quellen der Einträge sofort nach der Komprimierung eines Eintrags geschlossen werden sollen. |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Setzt die Kodierung zum Konvertieren von Dateinamen und anderen Zeichenketten in Bytes.

Falls nicht gesetzt, wird Codepage 437 verwendet.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.nio.charset.Charset | Kodierung zum Konvertieren von Dateinamen und anderen Zeichenketten in Bytes. |

### setEventsBag(EventsBag value) {#setEventsBag-com.aspose.zip.EventsBag-}
```
public final void setEventsBag(EventsBag value)
```


Setzt den Container von Ereignissen, die beim Speichern des Archivs ausgelöst werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [EventsBag](../../com.aspose.zip/eventsbag) | Container für Ereignisse, die beim Speichern des Archivs ausgelöst werden. |

