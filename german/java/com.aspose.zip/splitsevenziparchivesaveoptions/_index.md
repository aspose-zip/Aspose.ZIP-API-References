---
title: "SplitSevenZipArchiveSaveOptions"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Optionen zum Speichern eines mehrteiligen 7-Zip-Archivs."
type: docs
weight: 123
url: /de/java/com.aspose.zip/splitsevenziparchivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class SplitSevenZipArchiveSaveOptions
```

Optionen zum Speichern eines mehrteiligen 7-Zip-Archivs.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [SplitSevenZipArchiveSaveOptions(String fileName, long segmentSize)](#SplitSevenZipArchiveSaveOptions-java.lang.String-long-) | Instanziiert Einstellungen zum Speichern eines mehrteiligen 7z-Archivs. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getFileName()](#getFileName--) | Liefert den Namen der Segmente ohne Erweiterung. |
| [getSegmentSize()](#getSegmentSize--) | Liefert die Größe des Segments. |
### SplitSevenZipArchiveSaveOptions(String fileName, long segmentSize) {#SplitSevenZipArchiveSaveOptions-java.lang.String-long-}
```
public SplitSevenZipArchiveSaveOptions(String fileName, long segmentSize)
```


Instanziiert Einstellungen zum Speichern eines mehrteiligen 7z-Archivs.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | fileName | java.lang.String | Name für Volumen. Kann mit oder ohne .7z-Erweiterung sein. |

Dateinamen werden wie folgt sein: `fileName`.7z.001, `fileName`.7z.002, ..., `fileName`.7z.(n). |
|  | segmentSize | long | Größe des Volumens. |

Einige Volumen können kleiner als `segmentSize` sein. In den meisten Fällen ist das letzte Segment kleiner, aber selten können reguläre Segmente ebenfalls zu klein sein. |

### getFileName() {#getFileName--}
```
public final String getFileName()
```


Liefert den Namen der Segmente ohne Erweiterung.

**Returns:**
java.lang.String - der Name der Segmente ohne Erweiterung
### getSegmentSize() {#getSegmentSize--}
```
public final long getSegmentSize()
```


Liefert die Größe des Segments.

**Returns:**
long - die Größe des Segments.
