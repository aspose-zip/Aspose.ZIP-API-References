---
title: "ComHelper"
second_title: "Aspose.ZIP för Java API-referens"
description: "Tillhandahåller metoder för COM-klienter att ladda arkiv i Aspose.Zip."
type: docs
weight: 55
url: /sv/java/com.aspose.zip/comhelper/
---

**Inheritance:**
java.lang.Object
```
public class ComHelper
```

Tillhandahåller metoder för COM-klienter att ladda arkiv i Aspose.Zip.

Använd ComHelper-klassen för att läsa in ett arkiv från en fil eller ström. Specifika klasser tillhandahåller en standardkonstruktor för att skapa ett nytt arkiv och erbjuder även överlagrade konstruktorer för att läsa in ett arkiv från en fil eller ström. Om du använder Aspose.Zip från en .NET‑applikation kan du använda alla arkivkonstruktorer direkt, men om du använder Aspose.Zip från en COM‑applikation är endast standardkonstruktorn för arkivet tillgänglig.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [ComHelper()](#ComHelper--) | Initierar en ny instans av denna klass. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [openBzip2(InputStream stream)](#openBzip2-java.io.InputStream-) | Tillåter en COM‑applikation att läsa in ett bzip2‑arkiv från en ström. |
| [openBzip2(String fileName)](#openBzip2-java.lang.String-) | Tillåter en COM‑applikation att läsa in ett bzip2‑arkiv från en fil. |
| [openGzip(InputStream stream)](#openGzip-java.io.InputStream-) | Tillåter en COM‑applikation att läsa in ett gzip‑arkiv från en ström. |
| [openGzip(String fileName)](#openGzip-java.lang.String-) | Tillåter en COM‑applikation att läsa in ett gzip‑arkiv från en fil. |
| [openRar(InputStream stream)](#openRar-java.io.InputStream-) | Tillåter en COM‑applikation att läsa in ett rar‑arkiv från en ström. |
| [openRar(String fileName)](#openRar-java.lang.String-) | Tillåter en COM‑applikation att läsa in ett rar‑arkiv från en fil. |
| [openZip(InputStream stream)](#openZip-java.io.InputStream-) | Tillåter en COM‑applikation att läsa in ett ZIP‑arkiv från en ström. |
| [openZip(String fileName)](#openZip-java.lang.String-) | Tillåter en COM‑applikation att läsa in ett ZIP‑arkiv från en fil. |
### ComHelper() {#ComHelper--}
```
public ComHelper()
```


Initierar en ny instans av denna klass.

### openBzip2(InputStream stream) {#openBzip2-java.io.InputStream-}
```
public final Bzip2Archive openBzip2(InputStream stream)
```


Tillåter en COM‑applikation att läsa in ett bzip2‑arkiv från en ström.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | java.io.InputStream | Ett .NET‑strömobjekt som innehåller arkivet som ska läsas in. |

**Returns:**
[Bzip2Archive](../../com.aspose.zip/bzip2archive) - A [Bzip2Archive](../../com.aspose.zip/bzip2archive) object that represents the archive.
### openBzip2(String fileName) {#openBzip2-java.lang.String-}
```
public final Bzip2Archive openBzip2(String fileName)
```


Tillåter en COM‑applikation att läsa in ett bzip2‑arkiv från en fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | java.lang.String | Filnamn på arkivet som ska läsas in. |

**Returns:**
[Bzip2Archive](../../com.aspose.zip/bzip2archive) - A [Bzip2Archive](../../com.aspose.zip/bzip2archive) object that represents the archive.
### openGzip(InputStream stream) {#openGzip-java.io.InputStream-}
```
public final GzipArchive openGzip(InputStream stream)
```


Tillåter en COM‑applikation att läsa in ett gzip‑arkiv från en ström.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | java.io.InputStream | Ett .NET‑strömobjekt som innehåller arkivet som ska läsas in. |

**Returns:**
[GzipArchive](../../com.aspose.zip/gziparchive) - A [GzipArchive](../../com.aspose.zip/gziparchive) object that represents the archive.
### openGzip(String fileName) {#openGzip-java.lang.String-}
```
public final GzipArchive openGzip(String fileName)
```


Tillåter en COM‑applikation att läsa in ett gzip‑arkiv från en fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | java.lang.String | Filnamn på arkivet som ska läsas in. |

**Returns:**
[GzipArchive](../../com.aspose.zip/gziparchive) - A [GzipArchive](../../com.aspose.zip/gziparchive) object that represents the archive.
### openRar(InputStream stream) {#openRar-java.io.InputStream-}
```
public final RarArchive openRar(InputStream stream)
```


Tillåter en COM‑applikation att läsa in ett rar‑arkiv från en ström.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | java.io.InputStream | Ett .NET‑strömobjekt som innehåller arkivet som ska läsas in. |

**Returns:**
[RarArchive](../../com.aspose.zip/rararchive) - A [RarArchive](../../com.aspose.zip/rararchive) object that represents the archive.
### openRar(String fileName) {#openRar-java.lang.String-}
```
public final RarArchive openRar(String fileName)
```


Tillåter en COM‑applikation att läsa in ett rar‑arkiv från en fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | java.lang.String | Filnamn på arkivet som ska läsas in. |

**Returns:**
[RarArchive](../../com.aspose.zip/rararchive) - A [RarArchive](../../com.aspose.zip/rararchive) object that represents the archive.
### openZip(InputStream stream) {#openZip-java.io.InputStream-}
```
public final Archive openZip(InputStream stream)
```


Tillåter en COM‑applikation att läsa in ett ZIP‑arkiv från en ström.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | java.io.InputStream | Ett .NET‑strömobjekt som innehåller arkivet som ska läsas in. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - A [Archive](../../com.aspose.zip/archive) object that represents the archive.
### openZip(String fileName) {#openZip-java.lang.String-}
```
public final Archive openZip(String fileName)
```


Tillåter en COM‑applikation att läsa in ett ZIP‑arkiv från en fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | java.lang.String | Filnamn på arkivet som ska läsas in. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - A [Archive](../../com.aspose.zip/archive) object that represents the archive.
