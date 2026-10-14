---
title: "LzxArchive"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Diese Klasse repräsentiert eine LZX .lzx-Archivdatei."
type: docs
weight: 89
url: /de/java/com.aspose.zip/lzxarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class LzxArchive implements IArchive, AutoCloseable
```

Diese Klasse stellt eine LZX (.lzx)-Archivdatei dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [LzxArchive(InputStream extractionSource)](#LzxArchive-java.io.InputStream-) | Initialisiert eine neue Instanz der [LzxArchive](../../com.aspose.zip/lzxarchive)-Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann. |
| [LzxArchive(InputStream extractionSource, LzxLoadOptions loadOptions)](#LzxArchive-java.io.InputStream-com.aspose.zip.LzxLoadOptions-) | Initialisiert eine neue Instanz der [LzxArchive](../../com.aspose.zip/lzxarchive)-Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann. |
| [LzxArchive(String path)](#LzxArchive-java.lang.String-) | Initialisiert eine neue Instanz der [LzxArchive](../../com.aspose.zip/lzxarchive)-Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann. |
| [LzxArchive(String path, LzxLoadOptions loadOptions)](#LzxArchive-java.lang.String-com.aspose.zip.LzxLoadOptions-) | Initialisiert eine neue Instanz der [LzxArchive](../../com.aspose.zip/lzxarchive)-Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrahiert alle Dateien und Verzeichnisse im Archiv in das angegebene Verzeichnis. |
| [getEntries()](#getEntries--) | Liefert Dateieinträge vom Typ [LzxArchiveEntry](../../com.aspose.zip/lzxarchiveentry), die das Archiv bilden. |
| [getFileEntries()](#getFileEntries--) | Ruft Einträge vom Typ [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) ab, die das Archiv bilden. |
| [getFormat()](#getFormat--) | Liefert das Archivformat. |
### LzxArchive(InputStream extractionSource) {#LzxArchive-java.io.InputStream-}
```
public LzxArchive(InputStream extractionSource)
```


Initialisiert eine neue Instanz der [LzxArchive](../../com.aspose.zip/lzxarchive)-Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann.

Dieser Konstruktor dekomprimiert keinen Eintrag. Siehe die Methode [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\#extract-OutputStream-) zum Dekomprimieren.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| extractionSource | java.io.InputStream | Die Quelle des Archivs. |

### LzxArchive(InputStream extractionSource, LzxLoadOptions loadOptions) {#LzxArchive-java.io.InputStream-com.aspose.zip.LzxLoadOptions-}
```
public LzxArchive(InputStream extractionSource, LzxLoadOptions loadOptions)
```


Initialisiert eine neue Instanz der [LzxArchive](../../com.aspose.zip/lzxarchive)-Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann.

Dieser Konstruktor dekomprimiert keinen Eintrag. Siehe die Methode [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\#extract-OutputStream-) zum Dekomprimieren.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| extractionSource | java.io.InputStream | Die Quelle des Archivs. |
| loadOptions | [LzxLoadOptions](../../com.aspose.zip/lzxloadoptions) | Optionen zum Laden eines bestehenden Archivs. |

### LzxArchive(String path) {#LzxArchive-java.lang.String-}
```
public LzxArchive(String path)
```


Initialisiert eine neue Instanz der [LzxArchive](../../com.aspose.zip/lzxarchive)-Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann.

Das folgende Beispiel extrahiert ein Archiv und dekomprimiert anschließend den ersten Eintrag in einen `MemoryStream`.

```

``````

ByteArrayOutputStream extracted = new ByteArrayOutputStream();
try (LzxArchive archive = new LzxArchive("sample.lzx")) {
archive.getEntries().get(0).extract(extracted);
}
 
```

This constructor does not decompress any entry. See [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The fully qualified or the relative path to the archive file. |

### LzxArchive(String path, LzxLoadOptions loadOptions) {#LzxArchive-java.lang.String-com.aspose.zip.LzxLoadOptions-}
```
public LzxArchive(String path, LzxLoadOptions loadOptions)
```


Initializes a new instance of the [LzxArchive](../../com.aspose.zip/lzxarchive) class and composes an entry list can be extracted from the archive.

The following example extracts an archive, then decompress first entry to a `MemoryStream`.

```

``````

     ByteArrayOutputStream extracted = new ByteArrayOutputStream();
     try (LzxArchive archive = new LzxArchive("sample.lzx")) {
         archive.getEntries().get(0).extract(extracted);
     }
 
```

Dieser Konstruktor dekomprimiert keinen Eintrag. Siehe die Methode [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\#extract-OutputStream-) zum Dekomprimieren.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | java.lang.String | Der vollqualifizierte oder relative Pfad zur Archivdatei. |
| loadOptions | [LzxLoadOptions](../../com.aspose.zip/lzxloadoptions) | Optionen zum Laden eines bestehenden Archivs. |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extrahiert alle Dateien und Verzeichnisse im Archiv in das angegebene Verzeichnis.

```

``````

try (LzxArchive archive = new LzxArchive("archive.lzx")) {
archive.extractToDirectory("C:/extracted");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | The path to the directory to place the extracted files in.

If the directory does not exist, it will be created. |

### getEntries() {#getEntries--}
```
public final List<LzxArchiveEntry> getEntries()
```


Gets file entries of [LzxArchiveEntry](../../com.aspose.zip/lzxarchiveentry) type constituting the archive.

**Returns:**
java.util.List&lt;com.aspose.zip.LzxArchiveEntry&gt; - file entries of [LzxArchiveEntry](../../com.aspose.zip/lzxarchiveentry) type constituting the archive.
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the archive
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Gets the archive format.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
