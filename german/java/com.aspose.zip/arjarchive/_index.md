---
title: "ArjArchive"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Diese Klasse repräsentiert eine ARJ-Archivdatei."
type: docs
weight: 37
url: /de/java/com.aspose.zip/arjarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class ArjArchive implements IArchive, AutoCloseable
```

Diese Klasse repräsentiert eine ARJ-Archivdatei.

Nur die folgenden Komprimierungsmethoden werden unterstützt:

| ------ | ------------------------------------------------------------ |
| Method | Explanation                                                  |
| 0      | Unkomprimiert                                                 |
| 1      | Kombination aus LZ77 und adaptiver Huffman-Codierung. Bestes Verhältnis. |
| 2      | Kombination aus LZ77 und adaptiver Huffman-Codierung.             |
| 3      | Kombination aus LZ77 und adaptiver Huffman-Codierung. Beste Geschwindigkeit. |
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [ArjArchive(InputStream extractionSource)](#ArjArchive-java.io.InputStream-) | Initialisiert eine neue Instanz der [ArjArchive](../../com.aspose.zip/arjarchive)-Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann. |
| [ArjArchive(InputStream extractionSource, ArjLoadOptions loadOptions)](#ArjArchive-java.io.InputStream-com.aspose.zip.ArjLoadOptions-) | Initialisiert eine neue Instanz der [ArjArchive](../../com.aspose.zip/arjarchive)-Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann. |
| [ArjArchive(String path)](#ArjArchive-java.lang.String-) | Initialisiert eine neue Instanz der [ArjArchive](../../com.aspose.zip/arjarchive)-Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann. |
| [ArjArchive(String path, ArjLoadOptions loadOptions)](#ArjArchive-java.lang.String-com.aspose.zip.ArjLoadOptions-) | Initialisiert eine neue Instanz der [ArjArchive](../../com.aspose.zip/arjarchive)-Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrahiert alle Einträge in das angegebene Verzeichnis. |
| [getCommentary()](#getCommentary--) | Liefert den Kommentar. |
| [getEntries()](#getEntries--) | Liefert Einträge des Typs [ArjEntryPlain](../../com.aspose.zip/arjentryplain), die das ARJ-Archiv bilden. |
| [getFileEntries()](#getFileEntries--) | Ruft Einträge vom Typ [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) ab, die das Archiv bilden. |
| [getFormat()](#getFormat--) | Liefert das Archivformat. |
| [getName()](#getName--) | Liefert den Originalnamen. |
### ArjArchive(InputStream extractionSource) {#ArjArchive-java.io.InputStream-}
```
public ArjArchive(InputStream extractionSource)
```


Initialisiert eine neue Instanz der [ArjArchive](../../com.aspose.zip/arjarchive)-Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann.

Dieser Konstruktor dekomprimiert keinen Eintrag. Siehe die Methode [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\#extract-java.io.OutputStream-) zum Dekomprimieren.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| extractionSource | java.io.InputStream | die Quelle des Archivs |

### ArjArchive(InputStream extractionSource, ArjLoadOptions loadOptions) {#ArjArchive-java.io.InputStream-com.aspose.zip.ArjLoadOptions-}
```
public ArjArchive(InputStream extractionSource, ArjLoadOptions loadOptions)
```


Initialisiert eine neue Instanz der [ArjArchive](../../com.aspose.zip/arjarchive)-Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann.

Dieser Konstruktor dekomprimiert keinen Eintrag. Siehe die Methode [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\#extract-java.io.OutputStream-) zum Dekomprimieren.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| extractionSource | java.io.InputStream | die Quelle des Archivs |
| loadOptions | [ArjLoadOptions](../../com.aspose.zip/arjloadoptions) | Optionen zum Laden eines bestehenden Archivs. |

### ArjArchive(String path) {#ArjArchive-java.lang.String-}
```
public ArjArchive(String path)
```


Initialisiert eine neue Instanz der [ArjArchive](../../com.aspose.zip/arjarchive)-Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann.

Das folgende Beispiel zeigt, wie man alle Einträge in ein Verzeichnis extrahiert.

```

``````

try (ArjArchive archive = new ArjArchive("archive.arj")) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry. See [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\#extract-java.io.OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### ArjArchive(String path, ArjLoadOptions loadOptions) {#ArjArchive-java.lang.String-com.aspose.zip.ArjLoadOptions-}
```
public ArjArchive(String path, ArjLoadOptions loadOptions)
```


Initializes a new instance of the [ArjArchive](../../com.aspose.zip/arjarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (ArjArchive archive = new ArjArchive("archive.arj")) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

Dieser Konstruktor packt keinen Eintrag aus. Siehe die Methode [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\#extract-java.io.OutputStream-) zum Dekomprimieren.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | java.lang.String | der Pfad zur Archivdatei |
| loadOptions | [ArjLoadOptions](../../com.aspose.zip/arjloadoptions) | Optionen zum Laden eines bestehenden Archivs. |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extrahiert alle Einträge in das angegebene Verzeichnis.

Das folgende Beispiel zeigt, wie alle Einträge in ein Verzeichnis extrahiert werden können:

```

``````

try (ArjArchive archive = new ArjArchive(new FileInputStream("archive.arj"))) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the directory to extract the entries to |

### getCommentary() {#getCommentary--}
```
public final String getCommentary()
```


Gets the commentary.

**Returns:**
java.lang.String - the commentary.
### getEntries() {#getEntries--}
```
public final List<ArjEntryPlain> getEntries()
```


Gets entries of [ArjEntryPlain](../../com.aspose.zip/arjentryplain) type constituting the ARJ archive.

**Returns:**
java.util.List&lt;com.aspose.zip.ArjEntryPlain&gt; - entries of [ArjEntryPlain](../../com.aspose.zip/arjentryplain) type constituting the ARJ archive.
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
### getName() {#getName--}
```
public final String getName()
```


Gets the original name.

**Returns:**
java.lang.String - the original name.
