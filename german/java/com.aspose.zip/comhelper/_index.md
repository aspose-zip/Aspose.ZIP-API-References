---
title: "ComHelper"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Stellt Methoden für COM-Clients bereit, um Archive in Aspose.Zip zu laden."
type: docs
weight: 55
url: /de/java/com.aspose.zip/comhelper/
---

**Inheritance:**
java.lang.Object
```
public class ComHelper
```

Stellt Methoden für COM-Clients bereit, um Archive in Aspose.Zip zu laden.

Verwenden Sie die ComHelper-Klasse, um ein Archiv aus einer Datei oder einem Stream zu laden. Bestimmte Klassen stellen einen Standardkonstruktor bereit, um ein neues Archiv zu erstellen, und bieten außerdem überladene Konstruktoren zum Laden eines Archivs aus einer Datei oder einem Stream. Wenn Sie Aspose.Zip in einer .NET-Anwendung verwenden, können Sie alle Archivkonstruktoren direkt nutzen, aber wenn Sie Aspose.Zip in einer COM-Anwendung verwenden, ist nur der Standard-Archivkonstruktor verfügbar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [ComHelper()](#ComHelper--) | Initialisiert eine neue Instanz dieser Klasse. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [openBzip2(InputStream stream)](#openBzip2-java.io.InputStream-) | Ermöglicht einer COM-Anwendung, ein bzip2-Archiv aus einem Stream zu laden. |
| [openBzip2(String fileName)](#openBzip2-java.lang.String-) | Ermöglicht einer COM-Anwendung, ein bzip2-Archiv aus einer Datei zu laden. |
| [openGzip(InputStream stream)](#openGzip-java.io.InputStream-) | Ermöglicht einer COM-Anwendung, ein gzip-Archiv aus einem Stream zu laden. |
| [openGzip(String fileName)](#openGzip-java.lang.String-) | Ermöglicht einer COM-Anwendung, ein gzip-Archiv aus einer Datei zu laden. |
| [openRar(InputStream stream)](#openRar-java.io.InputStream-) | Ermöglicht einer COM-Anwendung, ein rar-Archiv aus einem Stream zu laden. |
| [openRar(String fileName)](#openRar-java.lang.String-) | Ermöglicht einer COM-Anwendung, ein rar-Archiv aus einer Datei zu laden. |
| [openZip(InputStream stream)](#openZip-java.io.InputStream-) | Ermöglicht einer COM-Anwendung, ein ZIP-Archiv aus einem Stream zu laden. |
| [openZip(String fileName)](#openZip-java.lang.String-) | Ermöglicht einer COM-Anwendung, ein ZIP-Archiv aus einer Datei zu laden. |
### ComHelper() {#ComHelper--}
```
public ComHelper()
```


Initialisiert eine neue Instanz dieser Klasse.

### openBzip2(InputStream stream) {#openBzip2-java.io.InputStream-}
```
public final Bzip2Archive openBzip2(InputStream stream)
```


Ermöglicht einer COM-Anwendung, ein bzip2-Archiv aus einem Stream zu laden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stream | java.io.InputStream | Ein .NET-Stream-Objekt, das das zu ladende Archiv enthält. |

**Returns:**
[Bzip2Archive](../../com.aspose.zip/bzip2archive) - A [Bzip2Archive](../../com.aspose.zip/bzip2archive) object that represents the archive.
### openBzip2(String fileName) {#openBzip2-java.lang.String-}
```
public final Bzip2Archive openBzip2(String fileName)
```


Ermöglicht einer COM-Anwendung, ein bzip2-Archiv aus einer Datei zu laden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | java.lang.String | Dateiname des Archivs, das geladen werden soll. |

**Returns:**
[Bzip2Archive](../../com.aspose.zip/bzip2archive) - A [Bzip2Archive](../../com.aspose.zip/bzip2archive) object that represents the archive.
### openGzip(InputStream stream) {#openGzip-java.io.InputStream-}
```
public final GzipArchive openGzip(InputStream stream)
```


Ermöglicht einer COM-Anwendung, ein gzip-Archiv aus einem Stream zu laden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stream | java.io.InputStream | Ein .NET-Stream-Objekt, das das zu ladende Archiv enthält. |

**Returns:**
[GzipArchive](../../com.aspose.zip/gziparchive) - A [GzipArchive](../../com.aspose.zip/gziparchive) object that represents the archive.
### openGzip(String fileName) {#openGzip-java.lang.String-}
```
public final GzipArchive openGzip(String fileName)
```


Ermöglicht einer COM-Anwendung, ein gzip-Archiv aus einer Datei zu laden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | java.lang.String | Dateiname des Archivs, das geladen werden soll. |

**Returns:**
[GzipArchive](../../com.aspose.zip/gziparchive) - A [GzipArchive](../../com.aspose.zip/gziparchive) object that represents the archive.
### openRar(InputStream stream) {#openRar-java.io.InputStream-}
```
public final RarArchive openRar(InputStream stream)
```


Ermöglicht einer COM-Anwendung, ein rar-Archiv aus einem Stream zu laden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stream | java.io.InputStream | Ein .NET-Stream-Objekt, das das zu ladende Archiv enthält. |

**Returns:**
[RarArchive](../../com.aspose.zip/rararchive) - A [RarArchive](../../com.aspose.zip/rararchive) object that represents the archive.
### openRar(String fileName) {#openRar-java.lang.String-}
```
public final RarArchive openRar(String fileName)
```


Ermöglicht einer COM-Anwendung, ein rar-Archiv aus einer Datei zu laden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | java.lang.String | Dateiname des Archivs, das geladen werden soll. |

**Returns:**
[RarArchive](../../com.aspose.zip/rararchive) - A [RarArchive](../../com.aspose.zip/rararchive) object that represents the archive.
### openZip(InputStream stream) {#openZip-java.io.InputStream-}
```
public final Archive openZip(InputStream stream)
```


Ermöglicht einer COM-Anwendung, ein ZIP-Archiv aus einem Stream zu laden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stream | java.io.InputStream | Ein .NET-Stream-Objekt, das das zu ladende Archiv enthält. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - A [Archive](../../com.aspose.zip/archive) object that represents the archive.
### openZip(String fileName) {#openZip-java.lang.String-}
```
public final Archive openZip(String fileName)
```


Ermöglicht einer COM-Anwendung, ein ZIP-Archiv aus einer Datei zu laden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | java.lang.String | Dateiname des Archivs, das geladen werden soll. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - A [Archive](../../com.aspose.zip/archive) object that represents the archive.
