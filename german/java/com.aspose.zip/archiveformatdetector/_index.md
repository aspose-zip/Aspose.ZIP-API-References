---
title: "ArchiveFormatDetector"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Erkennt ein Archivformat und liefert weitere zugehörige Informationen."
type: docs
weight: 32
url: /de/java/com.aspose.zip/archiveformatdetector/
---

**Inheritance:**
java.lang.Object
```
public final class ArchiveFormatDetector
```

Erkennt ein Archivformat und liefert weitere zugehörige Informationen.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [ArchiveFormatDetector()](#ArchiveFormatDetector--) | Initialisiert eine neue Instanz der [ArchiveFormatDetector](../../com.aspose.zip/archiveformatdetector) Klasse. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getFormatInfo(InputStream stream)](#getFormatInfo-java.io.InputStream-) | Ruft Formatinformationen ab. |
| [getFormatInfo(String fileName)](#getFormatInfo-java.lang.String-) | Ruft Formatinformationen ab. |
### ArchiveFormatDetector() {#ArchiveFormatDetector--}
```
public ArchiveFormatDetector()
```


Initialisiert eine neue Instanz der [ArchiveFormatDetector](../../com.aspose.zip/archiveformatdetector) Klasse.

### getFormatInfo(InputStream stream) {#getFormatInfo-java.io.InputStream-}
```
public final ArchiveFormatInfo getFormatInfo(InputStream stream)
```


Ruft Formatinformationen ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stream | java.io.InputStream | Der Stream der Archivdatei. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format or null if a format was not detected.
### getFormatInfo(String fileName) {#getFormatInfo-java.lang.String-}
```
public final ArchiveFormatInfo getFormatInfo(String fileName)
```


Ruft Formatinformationen ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | java.lang.String | Der Dateiname der Archivdatei. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format or null if a format was not detected.
