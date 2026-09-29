---
title: "ComHelper"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Biedt methoden voor COM-clients om archieven te laden in Aspose.Zip."
type: docs
weight: 55
url: /nl/java/com.aspose.zip/comhelper/
---

**Inheritance:**
java.lang.Object
```
public class ComHelper
```

Biedt methoden voor COM-clients om archieven te laden in Aspose.Zip.

Gebruik de ComHelper‑klasse om een archief uit een bestand of stream te laden. Bepaalde klassen bieden een standaardconstructor om een nieuw archief te maken en bieden ook overladen constructors om een archief uit een bestand of stream te laden. Als u Aspose.Zip gebruikt vanuit een .NET‑toepassing, kunt u alle archief‑constructors direct gebruiken, maar als u Aspose.Zip gebruikt vanuit een COM‑toepassing, is alleen de standaard‑archiefconstructor beschikbaar.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [ComHelper()](#ComHelper--) | Initialiseert een nieuw exemplaar van deze klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [openBzip2(InputStream stream)](#openBzip2-java.io.InputStream-) | Staat een COM‑applicatie toe een bzip2‑archief uit een stream te laden. |
| [openBzip2(String fileName)](#openBzip2-java.lang.String-) | Staat een COM‑applicatie toe een bzip2‑archief uit een bestand te laden. |
| [openGzip(InputStream stream)](#openGzip-java.io.InputStream-) | Staat een COM‑applicatie toe een gzip‑archief uit een stream te laden. |
| [openGzip(String fileName)](#openGzip-java.lang.String-) | Staat een COM‑applicatie toe een gzip‑archief uit een bestand te laden. |
| [openRar(InputStream stream)](#openRar-java.io.InputStream-) | Staat een COM‑applicatie toe een rar‑archief uit een stream te laden. |
| [openRar(String fileName)](#openRar-java.lang.String-) | Staat een COM‑applicatie toe een rar‑archief uit een bestand te laden. |
| [openZip(InputStream stream)](#openZip-java.io.InputStream-) | Staat een COM‑applicatie toe een ZIP‑archief uit een stream te laden. |
| [openZip(String fileName)](#openZip-java.lang.String-) | Staat een COM‑applicatie toe een ZIP‑archief uit een bestand te laden. |
### ComHelper() {#ComHelper--}
```
public ComHelper()
```


Initialiseert een nieuw exemplaar van deze klasse.

### openBzip2(InputStream stream) {#openBzip2-java.io.InputStream-}
```
public final Bzip2Archive openBzip2(InputStream stream)
```


Staat een COM‑applicatie toe een bzip2‑archief uit een stream te laden.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stream | java.io.InputStream | Een .NET‑streamobject dat het te laden archief bevat. |

**Returns:**
[Bzip2Archive](../../com.aspose.zip/bzip2archive) - A [Bzip2Archive](../../com.aspose.zip/bzip2archive) object that represents the archive.
### openBzip2(String fileName) {#openBzip2-java.lang.String-}
```
public final Bzip2Archive openBzip2(String fileName)
```


Staat een COM‑applicatie toe een bzip2‑archief uit een bestand te laden.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fileName | java.lang.String | Bestandsnaam van het archief om te laden. |

**Returns:**
[Bzip2Archive](../../com.aspose.zip/bzip2archive) - A [Bzip2Archive](../../com.aspose.zip/bzip2archive) object that represents the archive.
### openGzip(InputStream stream) {#openGzip-java.io.InputStream-}
```
public final GzipArchive openGzip(InputStream stream)
```


Staat een COM‑applicatie toe een gzip‑archief uit een stream te laden.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stream | java.io.InputStream | Een .NET‑streamobject dat het te laden archief bevat. |

**Returns:**
[GzipArchive](../../com.aspose.zip/gziparchive) - A [GzipArchive](../../com.aspose.zip/gziparchive) object that represents the archive.
### openGzip(String fileName) {#openGzip-java.lang.String-}
```
public final GzipArchive openGzip(String fileName)
```


Staat een COM‑applicatie toe een gzip‑archief uit een bestand te laden.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fileName | java.lang.String | Bestandsnaam van het archief om te laden. |

**Returns:**
[GzipArchive](../../com.aspose.zip/gziparchive) - A [GzipArchive](../../com.aspose.zip/gziparchive) object that represents the archive.
### openRar(InputStream stream) {#openRar-java.io.InputStream-}
```
public final RarArchive openRar(InputStream stream)
```


Staat een COM‑applicatie toe een rar‑archief uit een stream te laden.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stream | java.io.InputStream | Een .NET‑streamobject dat het te laden archief bevat. |

**Returns:**
[RarArchive](../../com.aspose.zip/rararchive) - A [RarArchive](../../com.aspose.zip/rararchive) object that represents the archive.
### openRar(String fileName) {#openRar-java.lang.String-}
```
public final RarArchive openRar(String fileName)
```


Staat een COM‑applicatie toe een rar‑archief uit een bestand te laden.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fileName | java.lang.String | Bestandsnaam van het archief om te laden. |

**Returns:**
[RarArchive](../../com.aspose.zip/rararchive) - A [RarArchive](../../com.aspose.zip/rararchive) object that represents the archive.
### openZip(InputStream stream) {#openZip-java.io.InputStream-}
```
public final Archive openZip(InputStream stream)
```


Staat een COM‑applicatie toe een ZIP‑archief uit een stream te laden.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stream | java.io.InputStream | Een .NET‑streamobject dat het te laden archief bevat. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - A [Archive](../../com.aspose.zip/archive) object that represents the archive.
### openZip(String fileName) {#openZip-java.lang.String-}
```
public final Archive openZip(String fileName)
```


Staat een COM‑applicatie toe een ZIP‑archief uit een bestand te laden.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fileName | java.lang.String | Bestandsnaam van het archief om te laden. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - A [Archive](../../com.aspose.zip/archive) object that represents the archive.
