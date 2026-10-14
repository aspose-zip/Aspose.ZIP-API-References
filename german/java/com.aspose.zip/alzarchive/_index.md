---
title: "AlzArchive"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Stellt eine ALZ-Archivdatei dar."
type: docs
weight: 11
url: /de/java/com.aspose.zip/alzarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class AlzArchive implements IArchive, AutoCloseable
```

Stellt eine ALZ-Archivdatei dar. Verwenden Sie diese Klasse, um ALZ-Archive zu untersuchen und zu extrahieren.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [AlzArchive(InputStream stream)](#AlzArchive-java.io.InputStream-) | Initialisiert ein ALZ-Archiv aus einem Stream. |
| [AlzArchive(InputStream stream, AlzArchiveLoadOptions loadOptions)](#AlzArchive-java.io.InputStream-com.aspose.zip.AlzArchiveLoadOptions-) | Initialisiert ein ALZ-Archiv aus einem Stream unter Verwendung der bereitgestellten Ladeoptionen. |
| [AlzArchive(String filePath)](#AlzArchive-java.lang.String-) | Initialisiert ein ALZ-Archiv aus einem Dateipfad. |
| [AlzArchive(String filePath, AlzArchiveLoadOptions loadOptions)](#AlzArchive-java.lang.String-com.aspose.zip.AlzArchiveLoadOptions-) | Initialisiert ein ALZ-Archiv aus einem Dateipfad unter Verwendung der bereitgestellten Ladeoptionen. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [close()](#close--) | Gibt Ressourcen frei, die von diesem Archiv gehalten werden. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrahiert alle Dateien und Verzeichnisse in das bereitgestellte Verzeichnis. |
| [getEntries()](#getEntries--) | Liefert die Einträge, die dieses Archiv bilden. |
| [getFileEntries()](#getFileEntries--) | Liefert Einträge über die gemeinsame Archivschnittstelle. |
| [getFormat()](#getFormat--) | Liefert das Archivformat. |
### AlzArchive(InputStream stream) {#AlzArchive-java.io.InputStream-}
```
public AlzArchive(InputStream stream)
```


Initialisiert ein ALZ-Archiv aus einem Stream.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stream | java.io.InputStream | ALZ archive stream; er muss Lesen und Suchen unterstützen |

### AlzArchive(InputStream stream, AlzArchiveLoadOptions loadOptions) {#AlzArchive-java.io.InputStream-com.aspose.zip.AlzArchiveLoadOptions-}
```
public AlzArchive(InputStream stream, AlzArchiveLoadOptions loadOptions)
```


Initialisiert ein ALZ-Archiv aus einem Stream unter Verwendung der bereitgestellten Ladeoptionen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stream | java.io.InputStream | ALZ archive stream; er muss Lesen und Suchen unterstützen |
| loadOptions | [AlzArchiveLoadOptions](../../com.aspose.zip/alzarchiveloadoptions) | Zum Laden des Archivs verwendete Optionen |

### AlzArchive(String filePath) {#AlzArchive-java.lang.String-}
```
public AlzArchive(String filePath)
```


Initialisiert ein ALZ-Archiv aus einem Dateipfad.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filePath | java.lang.String | Pfad zu einem ALZ-Archiv |

### AlzArchive(String filePath, AlzArchiveLoadOptions loadOptions) {#AlzArchive-java.lang.String-com.aspose.zip.AlzArchiveLoadOptions-}
```
public AlzArchive(String filePath, AlzArchiveLoadOptions loadOptions)
```


Initialisiert ein ALZ-Archiv aus einem Dateipfad unter Verwendung der bereitgestellten Ladeoptionen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filePath | java.lang.String | Pfad zu einem ALZ-Archiv |
| loadOptions | [AlzArchiveLoadOptions](../../com.aspose.zip/alzarchiveloadoptions) | Zum Laden des Archivs verwendete Optionen |

### close() {#close--}
```
public void close()
```


Gibt Ressourcen frei, die von diesem Archiv gehalten werden.

### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extrahiert alle Dateien und Verzeichnisse in das bereitgestellte Verzeichnis.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| destinationDirectory | java.lang.String | Zielverzeichnis; es wird bei Bedarf erstellt |

### getEntries() {#getEntries--}
```
public final List<AlzEntry> getEntries()
```


Liefert die Einträge, die dieses Archiv bilden.

**Returns:**
java.util.List&lt;com.aspose.zip.AlzEntry&gt; - unveränderliche Liste von ALZ-Einträgen
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Liefert Einträge über die gemeinsame Archivschnittstelle.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - Archiv-Einträge
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Liefert das Archivformat.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - [ArchiveFormat.Alz](../../com.aspose.zip/archiveformat\#Alz)
