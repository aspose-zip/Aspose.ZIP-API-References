---
title: "SplitSevenZipArchiveSaveOptions"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Opties voor het opslaan van een multi-volume 7-zip-archief."
type: docs
weight: 123
url: /nl/java/com.aspose.zip/splitsevenziparchivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class SplitSevenZipArchiveSaveOptions
```

Opties voor het opslaan van een multi-volume 7-zip-archief.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [SplitSevenZipArchiveSaveOptions(String fileName, long segmentSize)](#SplitSevenZipArchiveSaveOptions-java.lang.String-long-) | Instantieert instellingen voor het opslaan van een multi-volume 7z-archief. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getFileName()](#getFileName--) | Haalt de naam van segmenten op zonder extensie. |
| [getSegmentSize()](#getSegmentSize--) | Haalt de grootte van het segment op. |
### SplitSevenZipArchiveSaveOptions(String fileName, long segmentSize) {#SplitSevenZipArchiveSaveOptions-java.lang.String-long-}
```
public SplitSevenZipArchiveSaveOptions(String fileName, long segmentSize)
```


Instantieert instellingen voor het opslaan van een multi-volume 7z-archief.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | fileName | java.lang.String | naam voor volumes. Kan met of zonder .7z-extensie zijn. |

Bestandsnamen zullen als volgt zijn: `fileName`.7z.001, `fileName`.7z.002, ..., `fileName`.7z.(n). |
|  | segmentSize | long | grootte van volume. |

Sommige volumes kunnen kleiner zijn dan `segmentSize`. In de meeste gevallen zal het laatste segment kleiner zijn, maar zelden kunnen reguliere segmenten ook te klein zijn. |

### getFileName() {#getFileName--}
```
public final String getFileName()
```


Haalt de naam van segmenten op zonder extensie.

**Returns:**
java.lang.String - de naam van segmenten zonder extensie
### getSegmentSize() {#getSegmentSize--}
```
public final long getSegmentSize()
```


Haalt de grootte van het segment op.

**Returns:**
long - de grootte van het segment.
