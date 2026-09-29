---
title: "SplitArchiveSaveOptions"
second_title: "Aspose.ZIP för Java API-referens"
description: "Alternativ för att spara ett flervolymigt ZIP-arkiv."
type: docs
weight: 122
url: /sv/java/com.aspose.zip/splitarchivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class SplitArchiveSaveOptions
```

Alternativ för att spara ett flervolymigt ZIP-arkiv.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [SplitArchiveSaveOptions(String fileName, long segmentSize)](#SplitArchiveSaveOptions-java.lang.String-long-) | Instansierar inställningar för att spara ett flervolym ZIP-arkiv. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getArchiveComment()](#getArchiveComment--) | Hämtar valfri kommentar för Zip-filen. |
| [getCloseEntrySource()](#getCloseEntrySource--) | Hämtar ett värde som indikerar om källorna för poster ska stängas omedelbart efter att en post har komprimerats. |
| [getEncoding()](#getEncoding--) | Hämtar kodning för att konvertera filnamn och andra strängar till byte. |
| [getEventsBag()](#getEventsBag--) | Hämtar behållare för händelser som utlöses vid arkivsparning. |
| [getFileName()](#getFileName--) | Hämtar namnet på segmenten utan filändelse. |
| [getSegmentSize()](#getSegmentSize--) | Hämtar storleken på segmentet. |
| [setArchiveComment(String value)](#setArchiveComment-java.lang.String-) | Ställer in valfri kommentar för Zip-filen. |
| [setCloseEntrySource(boolean value)](#setCloseEntrySource-boolean-) | Ställer in ett värde som indikerar om källorna för poster ska stängas omedelbart efter att en post har komprimerats. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Ställer in kodning för att konvertera filnamn och andra strängar till byte. |
| [setEventsBag(EventsBag value)](#setEventsBag-com.aspose.zip.EventsBag-) | Ställer in behållare för händelser som utlöses vid arkivsparning. |
### SplitArchiveSaveOptions(String fileName, long segmentSize) {#SplitArchiveSaveOptions-java.lang.String-long-}
```
public SplitArchiveSaveOptions(String fileName, long segmentSize)
```


Instansierar inställningar för att spara ett flervolym ZIP-arkiv.

Vissa volymer kan vara mindre än `segmentSize`. I de flesta fall kommer det sista segmentet att vara mindre, men sällan kan vanliga segment vara för stora.

Filnamn kommer att vara enligt följande: `fileName`.z01, `fileName`.z02, ..., `fileName`.z(n-1), `fileName`.zip.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | java.lang.String | Namn för volymer. Kan vara med eller utan .zip‑ändelse. |
| segmentSize | long | Storlek på volym. |

### getArchiveComment() {#getArchiveComment--}
```
public final String getArchiveComment()
```


Hämtar valfri kommentar för Zip-filen.

**Returns:**
java.lang.String - valfri kommentar för Zip-filen.
### getCloseEntrySource() {#getCloseEntrySource--}
```
public final boolean getCloseEntrySource()
```


Hämtar ett värde som indikerar om källorna för poster ska stängas omedelbart efter att en post har komprimerats.

**Returns:**
boolean - ett värde som indikerar om källorna för poster ska stängas direkt efter att en post har komprimerats.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Hämtar kodning för att konvertera filnamn och andra strängar till byte.

Om den inte är angiven används kodsidan 437.

**Returns:**
java.nio.charset.Charset - kodning för att konvertera filnamn och andra strängar till byte.
### getEventsBag() {#getEventsBag--}
```
public final EventsBag getEventsBag()
```


Hämtar behållare för händelser som utlöses vid arkivsparning.

**Returns:**
[EventsBag](../../com.aspose.zip/eventsbag) - container of events raising on archive saving.
### getFileName() {#getFileName--}
```
public final String getFileName()
```


Hämtar namnet på segmenten utan filändelse.

**Returns:**
java.lang.String – namnet på segmenten utan filändelse.
### getSegmentSize() {#getSegmentSize--}
```
public final long getSegmentSize()
```


Hämtar storleken på segmentet.

**Returns:**
long – storleken på segmentet.
### setArchiveComment(String value) {#setArchiveComment-java.lang.String-}
```
public final void setArchiveComment(String value)
```


Ställer in valfri kommentar för Zip-filen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | valfri kommentar för Zip‑filen. |

### setCloseEntrySource(boolean value) {#setCloseEntrySource-boolean-}
```
public final void setCloseEntrySource(boolean value)
```


Ställer in ett värde som indikerar om källorna för poster ska stängas omedelbart efter att en post har komprimerats.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om posternas källor ska stängas omedelbart efter att en post har komprimerats. |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Ställer in kodning för att konvertera filnamn och andra strängar till byte.

Om den inte är angiven används kodsidan 437.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.nio.charset.Charset | kodning för att konvertera filnamn och andra strängar till byte. |

### setEventsBag(EventsBag value) {#setEventsBag-com.aspose.zip.EventsBag-}
```
public final void setEventsBag(EventsBag value)
```


Ställer in behållare för händelser som utlöses vid arkivsparning.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [EventsBag](../../com.aspose.zip/eventsbag) | behållare för händelser som utlöses vid arkivlagring. |

