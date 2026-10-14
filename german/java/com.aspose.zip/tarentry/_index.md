---
title: "TarEntry"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Stellt eine einzelne Datei innerhalb eines Tar-Archivs dar."
type: docs
weight: 126
url: /de/java/com.aspose.zip/tarentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class TarEntry implements IArchiveFileEntry
```

Stellt eine einzelne Datei innerhalb eines Tar-Archivs dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrahiert den Eintrag in den bereitgestellten Stream. |
| [extract(String path)](#extract-java.lang.String-) | Extrahiert den Eintrag in das Dateisystem über den angegebenen Pfad. |
| [getLength()](#getLength--) | Gibt die Länge des Eintrags in Bytes zurück. |
| [getModificationTime()](#getModificationTime--) | Liefert den Änderungszeitpunkt der Datei oder des Verzeichnisses. |
| [getName()](#getName--) | Gibt den Namen des Eintrags im Archiv zurück. |
| [getUncompressedSize()](#getUncompressedSize--) | Liefert die Größe einer Originaldatei. |
| [isDirectory()](#isDirectory--) | Liefert einen Wert, der angibt, ob der Eintrag ein Verzeichnis darstellt. |
| [open()](#open--) | Öffnet den Eintrag zum Extrahieren und stellt einen Stream mit dem Eintragsinhalt bereit. |
| [setName(String value)](#setName-java.lang.String-) | Setzt den Namen des Eintrags im Archiv. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extrahiert den Eintrag in den bereitgestellten Stream.

Extrahiere einen Eintrag aus dem Tar-Archiv.

```

``````

try (TarArchive archive = new TarArchive(\"archive.tar\")) {
archive.getEntries().get_Item(0).extract(httpResponseStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | Destination stream. Must be writable. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the entry to the filesystem by the path provided.

```

``````

     try (TarArchive archive = new TarArchive("archive.tar")) {
         archive.getEntries().get_Item(0).extract("data.bin");
     }
 
```



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | java.lang.String | Der Pfad zur Zieldatei. Wenn die Datei bereits existiert, wird sie überschrieben. |

**Returns:**
java.io.File - die Dateiinformation der extrahierten Datei
### getLength() {#getLength--}
```
public final Long getLength()
```


Gibt die Länge des Eintrags in Bytes zurück.

**Returns:**
java.lang.Long – die Länge des Eintrags in Bytes
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Liefert den Änderungszeitpunkt der Datei oder des Verzeichnisses.

**Returns:**
java.util.Date - die Änderungszeit der Datei oder des Verzeichnisses.
### getName() {#getName--}
```
public final String getName()
```


Gibt den Namen des Eintrags im Archiv zurück.

**Returns:**
java.lang.String - der Name des Eintrags im Archiv
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Liefert die Größe einer Originaldatei.

Hat denselben Wert wie `Length`([getLength](../../com.aspose.zip/tarentry\#getLength--))

**Returns:**
long - die Größe einer Originaldatei.
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Liefert einen Wert, der angibt, ob der Eintrag ein Verzeichnis darstellt.

**Returns:**
boolean - ein Wert, der angibt, ob der Eintrag ein Verzeichnis darstellt
### open() {#open--}
```
public final InputStream open()
```


Öffnet den Eintrag zum Extrahieren und stellt einen Stream mit dem Eintragsinhalt bereit.


Verwendung:

```

``````

InputStream decompressed = entry.open();
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
fileStream.write(buffer, 0, bytesRead);
}
 
```

Read from the stream to get the original content of the file. See examples section.

**Returns:**
java.io.InputStream - the stream that represents the contents of the entry
### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Sets the name of the entry within the archive.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the name of the entry within the archive |

