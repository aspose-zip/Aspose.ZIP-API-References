---
title: "SplitSevenZipArchiveSaveOptions"
second_title: "Aspose.ZIP för Java API-referens"
description: "Alternativ för att spara ett flervolymigt 7-zip-arkiv."
type: docs
weight: 123
url: /sv/java/com.aspose.zip/splitsevenziparchivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class SplitSevenZipArchiveSaveOptions
```

Alternativ för att spara ett flervolymigt 7-zip-arkiv.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [SplitSevenZipArchiveSaveOptions(String fileName, long segmentSize)](#SplitSevenZipArchiveSaveOptions-java.lang.String-long-) | Instansierar inställningar för att spara ett flervolym 7z‑arkiv. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getFileName()](#getFileName--) | Hämtar namnet på segmenten utan filändelse. |
| [getSegmentSize()](#getSegmentSize--) | Hämtar storleken på segmentet. |
### SplitSevenZipArchiveSaveOptions(String fileName, long segmentSize) {#SplitSevenZipArchiveSaveOptions-java.lang.String-long-}
```
public SplitSevenZipArchiveSaveOptions(String fileName, long segmentSize)
```


Instansierar inställningar för att spara ett flervolym 7z‑arkiv.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | fileName | java.lang.String | namn för volymer. Kan vara med eller utan .7z‑ändelse. |

Filnamn kommer att vara enligt följande: `fileName`.7z.001, `fileName`.7z.002, ..., `fileName`.7z.(n). |
|  | segmentSize | long | storlek på volymen. |

Vissa volymer kan vara mindre än `segmentSize`. I de flesta fall kommer det sista segmentet att vara mindre, men sällan kan vanliga segment också vara det. |

### getFileName() {#getFileName--}
```
public final String getFileName()
```


Hämtar namnet på segmenten utan filändelse.

**Returns:**
java.lang.String – namnet på segmenten utan filändelse
### getSegmentSize() {#getSegmentSize--}
```
public final long getSegmentSize()
```


Hämtar storleken på segmentet.

**Returns:**
long – storleken på segmentet.
