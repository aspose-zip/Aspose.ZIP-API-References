---
title: "LhaArchive"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Diese Klasse repräsentiert eine LHA .lzh-Archivdatei."
type: docs
weight: 75
url: /de/java/com.aspose.zip/lhaarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class LhaArchive implements IArchive, AutoCloseable
```

Diese Klasse stellt eine LHA (.lzh)-Archivdatei dar.

Nur die folgenden Komprimierungsmethoden werden unterstützt:

| ------ | --------------------------------------------- |
| Methode | Erklärung                                   |
| lh0    | Unkomprimiert                                  |
| lh4    | 8 KiB Gleitendes Wörterbuch und statischer Huffman   |
| lh5    | 16 KiB Gleitendes Wörterbuch und statischer Huffman  |
| lh6    | 64 KiB Gleitendes Wörterbuch und statischer Huffman  |
| lh7    | 128 KiB Gleitendes Wörterbuch und statischer Huffman |
| lhx    | 1 Mib Gleitendes Wörterbuch und statischer Huffman   |
| lhd    | Verzeichnis                                     |
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [LhaArchive(InputStream sourceStream)](#LhaArchive-java.io.InputStream-) | Initialisiert eine neue Instanz der Klasse [LhaArchive](../../com.aspose.zip/lhaarchive) und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann. |
| [LhaArchive(InputStream sourceStream, LhaLoadOptions loadOptions)](#LhaArchive-java.io.InputStream-com.aspose.zip.LhaLoadOptions-) | Initialisiert eine neue Instanz der Klasse [LhaArchive](../../com.aspose.zip/lhaarchive) und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann. |
| [LhaArchive(String path)](#LhaArchive-java.lang.String-) | Initialisiert eine neue Instanz der Klasse [LhaArchive](../../com.aspose.zip/lhaarchive) und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann. |
| [LhaArchive(String path, LhaLoadOptions loadOptions)](#LhaArchive-java.lang.String-com.aspose.zip.LhaLoadOptions-) | Initialisiert eine neue Instanz der Klasse [LhaArchive](../../com.aspose.zip/lhaarchive) und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrahiert alle Dateien und Verzeichnisse im Archiv in das angegebene Verzeichnis. |
| [getEntries()](#getEntries--) | Gibt Dateieinträge des Typs [LhaArchiveEntry](../../com.aspose.zip/lhaarchiveentry) zurück, die das Archiv bilden. |
| [getFileEntries()](#getFileEntries--) | Ruft Einträge vom Typ [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) ab, die das Archiv bilden. |
| [getFormat()](#getFormat--) | Liefert das Archivformat. |
### LhaArchive(InputStream sourceStream) {#LhaArchive-java.io.InputStream-}
```
public LhaArchive(InputStream sourceStream)
```


Initialisiert eine neue Instanz der Klasse [LhaArchive](../../com.aspose.zip/lhaarchive) und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann.

Dieser Konstruktor dekomprimiert keinen Eintrag. Siehe die Methode [LhaArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lhaarchiveentry\#extract-OutputStream-) zum Dekomprimieren.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceStream | java.io.InputStream | die Quelle des Archivs |

### LhaArchive(InputStream sourceStream, LhaLoadOptions loadOptions) {#LhaArchive-java.io.InputStream-com.aspose.zip.LhaLoadOptions-}
```
public LhaArchive(InputStream sourceStream, LhaLoadOptions loadOptions)
```


Initialisiert eine neue Instanz der Klasse [LhaArchive](../../com.aspose.zip/lhaarchive) und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann.

Dieser Konstruktor dekomprimiert keinen Eintrag. Siehe die Methode [LhaArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lhaarchiveentry\#extract-OutputStream-) zum Dekomprimieren.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceStream | java.io.InputStream | die Quelle des Archivs |
| loadOptions | [LhaLoadOptions](../../com.aspose.zip/lhaloadoptions) | Optionen zum Laden eines bestehenden Archivs. |

### LhaArchive(String path) {#LhaArchive-java.lang.String-}
```
public LhaArchive(String path)
```


Initialisiert eine neue Instanz der Klasse [LhaArchive](../../com.aspose.zip/lhaarchive) und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann.

Das folgende Beispiel extrahiert ein Archiv und dekomprimiert anschließend den ersten Eintrag in einen `MemoryStream`.

```

``````

ByteArrayOutputStream extracted = new ByteArrayOutputStream();
try (LhaArchive archive = new LhaArchive("sample.lzh")) {
archive.getEntries().get(0).extract(extracted);
}
 
```

This constructor does not decompress any entry. See [ArchiveEntry.extract(OutputStream)](../../com.aspose.zip/archiveentry\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the fully qualified or the relative path to the archive file |

### LhaArchive(String path, LhaLoadOptions loadOptions) {#LhaArchive-java.lang.String-com.aspose.zip.LhaLoadOptions-}
```
public LhaArchive(String path, LhaLoadOptions loadOptions)
```


Initializes a new instance of the [LhaArchive](../../com.aspose.zip/lhaarchive) class and composes an entry list can be extracted from the archive.

The following example extracts an archive, then decompress first entry to a `MemoryStream`.

```

``````

     ByteArrayOutputStream extracted = new ByteArrayOutputStream();
     try (LhaArchive archive = new LhaArchive("sample.lzh")) {
         archive.getEntries().get(0).extract(extracted);
     }
 
```

Dieser Konstruktor dekomprimiert keinen Eintrag. Siehe die Methode [ArchiveEntry.extract(OutputStream)](../../com.aspose.zip/archiveentry\\#extract-OutputStream-) zum Dekomprimieren.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | java.lang.String | Der vollqualifizierte oder relative Pfad zur Archivdatei. |
| loadOptions | [LhaLoadOptions](../../com.aspose.zip/lhaloadoptions) | Optionen zum Laden eines bestehenden Archivs. |

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

try (LhaArchive archive = new LhaArchive(\"archive.lzh\")) {
archive.extractToDirectory("C:/extracted");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in.

If the directory does not exist, it will be created |

### getEntries() {#getEntries--}
```
public final List<LhaArchiveEntry> getEntries()
```


Gets file entries of [LhaArchiveEntry](../../com.aspose.zip/lhaarchiveentry) type constituting the archive.

**Returns:**
java.util.List&lt;com.aspose.zip.LhaArchiveEntry&gt; - file entries of [LhaArchiveEntry](../../com.aspose.zip/lhaarchiveentry) type constituting the archive
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
