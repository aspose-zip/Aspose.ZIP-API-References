---
title: "CpioEntry"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Stellt eine einzelne Datei innerhalb eines cpio-Archivs dar."
type: docs
weight: 58
url: /de/java/com.aspose.zip/cpioentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public final class CpioEntry implements IArchiveFileEntry
```

Stellt eine einzelne Datei innerhalb eines cpio-Archivs dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrahiert den Eintrag in den bereitgestellten Stream. |
| [extract(String path)](#extract-java.lang.String-) | Extrahiert den Eintrag in das Dateisystem über den angegebenen Pfad. |
| [getLastWriteTimeUtc()](#getLastWriteTimeUtc--) | Gibt die letzte Schreibzeit zurück. |
| [getLength()](#getLength--) | Gibt die Länge des Eintrags in Bytes zurück. |
| [getName()](#getName--) | Gibt den Namen des Eintrags im Archiv zurück. |
| [getParent()](#getParent--) | Gibt das Archiv zurück, zu dem der Eintrag gehört. |
| [isDirectory()](#isDirectory--) | Liefert einen Wert, der angibt, ob der Eintrag ein Verzeichnis darstellt. |
| [open()](#open--) | Öffnet den Eintrag zum Extrahieren und stellt einen Stream mit dem Eintragsinhalt bereit. |
| [toString()](#toString--) | Gibt die Zeichenkettenrepräsentation der Instanz der Klasse [CpioEntry](../../com.aspose.zip/cpioentry) zurück. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extrahiert den Eintrag in den bereitgestellten Stream.

Extrahiert einen Eintrag aus einem Cpio-Archiv.

```

``````

try (CpioArchive archive = new CpioArchive("archive.cpio")) {
archive.getEntries().get(0).extract(httpResponseStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream. Must be writable |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the entry to the filesystem by the path provided.

```

``````

     try (CpioArchive archive = new CpioArchive("archive.cpio")) {
         archive.getEntries().get(0).extract("data.bin");
     }
 
```



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | java.lang.String | Der Pfad zur Zieldatei. Wenn die Datei bereits existiert, wird sie überschrieben. |

**Returns:**
java.io.File - die Dateiinformation der extrahierten Datei
### getLastWriteTimeUtc() {#getLastWriteTimeUtc--}
```
public final Date getLastWriteTimeUtc()
```


Gibt die letzte Schreibzeit zurück.

**Returns:**
java.util.Date - die letzte Schreibzeit
### getLength() {#getLength--}
```
public final Long getLength()
```


Gibt die Länge des Eintrags in Bytes zurück.

**Returns:**
java.lang.Long – die Länge des Eintrags in Bytes
### getName() {#getName--}
```
public final String getName()
```


Gibt den Namen des Eintrags im Archiv zurück.

**Returns:**
java.lang.String - der Name des Eintrags im Archiv
### getParent() {#getParent--}
```
public final CpioArchive getParent()
```


Gibt das Archiv zurück, zu dem der Eintrag gehört.

**Returns:**
[CpioArchive](../../com.aspose.zip/cpioarchive) - the archive the entry belongs to
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Liefert einen Wert, der angibt, ob der Eintrag ein Verzeichnis darstellt.

**Returns:**
boolean - ein Wert, der angibt, ob der Eintrag ein Verzeichnis darstellt.
### open() {#open--}
```
public final InputStream open()
```


Öffnet den Eintrag zum Extrahieren und stellt einen Stream mit dem Eintragsinhalt bereit.

Verwendung:

```

``````

CpioArchive archive = new CpioArchive("archive.cpio");
CpioEntry entry = archive.getEntries().get(0);
try (FileOutputStream fileStream = new FileOutputStream("data.bin")) {
try (InputStream decompressed = entry.open()) {
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
fileStream.write(buffer, 0, bytesRead);
}
}
} catch (IOException ex) {
}
 
```

Read from the stream to get the original content of a file. See examples section.

**Returns:**
java.io.InputStream - the stream that represents the contents of the entry
### toString() {#toString--}
```
public String toString()
```


Returns string representation of the instance of the [CpioEntry](../../com.aspose.zip/cpioentry) class.

**Returns:**
java.lang.String - string representation of this object.
