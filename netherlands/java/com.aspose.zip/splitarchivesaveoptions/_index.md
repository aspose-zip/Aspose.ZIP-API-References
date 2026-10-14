---
title: "SplitArchiveSaveOptions"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Opties voor het opslaan van een multi-volume ZIP-archief."
type: docs
weight: 122
url: /nl/java/com.aspose.zip/splitarchivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class SplitArchiveSaveOptions
```

Opties voor het opslaan van een multi-volume ZIP-archief.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [SplitArchiveSaveOptions(String fileName, long segmentSize)](#SplitArchiveSaveOptions-java.lang.String-long-) | Instantieert instellingen voor het opslaan van een multi-volume ZIP-archief. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getArchiveComment()](#getArchiveComment--) | Haalt optionele opmerking op voor het Zip‑bestand. |
| [getCloseEntrySource()](#getCloseEntrySource--) | Haalt een waarde op die aangeeft of de bronnen van items direct na compressie van een item moeten worden gesloten. |
| [getEncoding()](#getEncoding--) | Haalt codering op voor het converteren van bestandsnamen en andere tekenreeksen naar bytes. |
| [getEventsBag()](#getEventsBag--) | Haalt container van gebeurtenissen op die worden geactiveerd bij het opslaan van een archief. |
| [getFileName()](#getFileName--) | Haalt de naam van segmenten op zonder extensie. |
| [getSegmentSize()](#getSegmentSize--) | Haalt de grootte van het segment op. |
| [setArchiveComment(String value)](#setArchiveComment-java.lang.String-) | Stelt optionele opmerking in voor het Zip‑bestand. |
| [setCloseEntrySource(boolean value)](#setCloseEntrySource-boolean-) | Stelt een waarde in die aangeeft of de bronnen van items direct na compressie van een item moeten worden gesloten. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Stelt codering in voor het converteren van bestandsnamen en andere tekenreeksen naar bytes. |
| [setEventsBag(EventsBag value)](#setEventsBag-com.aspose.zip.EventsBag-) | Stelt container van gebeurtenissen in die worden geactiveerd bij het opslaan van een archief. |
### SplitArchiveSaveOptions(String fileName, long segmentSize) {#SplitArchiveSaveOptions-java.lang.String-long-}
```
public SplitArchiveSaveOptions(String fileName, long segmentSize)
```


Instantieert instellingen voor het opslaan van een multi-volume ZIP-archief.

Sommige volumes kunnen kleiner zijn dan `segmentSize`. In de meeste gevallen zal het laatste segment kleiner zijn, maar zelden kunnen reguliere segmenten ook te klein zijn.

Bestandsnamen zullen als volgt zijn: `fileName`.z01, `fileName`.z02, ..., `fileName`.z(n-1), `fileName`.zip.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fileName | java.lang.String | Naam voor volumes. Kan met of zonder .zip-extensie zijn. |
| segmentSize | long | Grootte van volume. |

### getArchiveComment() {#getArchiveComment--}
```
public final String getArchiveComment()
```


Haalt optionele opmerking op voor het Zip‑bestand.

**Returns:**
java.lang.String - optionele opmerking voor het Zip-bestand.
### getCloseEntrySource() {#getCloseEntrySource--}
```
public final boolean getCloseEntrySource()
```


Haalt een waarde op die aangeeft of de bronnen van items direct na compressie van een item moeten worden gesloten.

**Returns:**
boolean - een waarde die aangeeft of de bronnen van items moeten worden gesloten direct nadat een item is gecomprimeerd.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Haalt codering op voor het converteren van bestandsnamen en andere tekenreeksen naar bytes.

Indien niet ingesteld, wordt codepagina 437 gebruikt.

**Returns:**
java.nio.charset.Charset - codering voor het converteren van bestandsnamen en andere strings naar bytes.
### getEventsBag() {#getEventsBag--}
```
public final EventsBag getEventsBag()
```


Haalt container van gebeurtenissen op die worden geactiveerd bij het opslaan van een archief.

**Returns:**
[EventsBag](../../com.aspose.zip/eventsbag) - container of events raising on archive saving.
### getFileName() {#getFileName--}
```
public final String getFileName()
```


Haalt de naam van segmenten op zonder extensie.

**Returns:**
java.lang.String - de naam van segmenten zonder extensie.
### getSegmentSize() {#getSegmentSize--}
```
public final long getSegmentSize()
```


Haalt de grootte van het segment op.

**Returns:**
long - de grootte van het segment.
### setArchiveComment(String value) {#setArchiveComment-java.lang.String-}
```
public final void setArchiveComment(String value)
```


Stelt optionele opmerking in voor het Zip‑bestand.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | optionele opmerking voor het Zip-bestand. |

### setCloseEntrySource(boolean value) {#setCloseEntrySource-boolean-}
```
public final void setCloseEntrySource(boolean value)
```


Stelt een waarde in die aangeeft of de bronnen van items direct na compressie van een item moeten worden gesloten.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of de bronnen van items direct na het comprimeren van een item moeten worden gesloten. |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Stelt codering in voor het converteren van bestandsnamen en andere tekenreeksen naar bytes.

Indien niet ingesteld, wordt codepagina 437 gebruikt.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.nio.charset.Charset | codering voor het converteren van bestandsnamen en andere strings naar bytes. |

### setEventsBag(EventsBag value) {#setEventsBag-com.aspose.zip.EventsBag-}
```
public final void setEventsBag(EventsBag value)
```


Stelt container van gebeurtenissen in die worden geactiveerd bij het opslaan van een archief.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [EventsBag](../../com.aspose.zip/eventsbag) | container van gebeurtenissen die worden getriggerd bij het opslaan van een archief. |

