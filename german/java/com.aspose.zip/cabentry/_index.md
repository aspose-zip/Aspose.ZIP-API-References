---
title: "CabEntry"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Stellt eine einzelne Datei innerhalb eines CAB-Archivs dar."
type: docs
weight: 46
url: /de/java/com.aspose.zip/cabentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public final class CabEntry implements IArchiveFileEntry
```

Stellt eine einzelne Datei innerhalb eines CAB-Archivs dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrahiert den Eintrag in den bereitgestellten Stream. |
| [extract(String path)](#extract-java.lang.String-) | Extrahiert den Eintrag in das Dateisystem über den angegebenen Pfad. |
| [getLength()](#getLength--) | Gibt die Länge des Eintrags in Bytes zurück. |
| [getModificationTime()](#getModificationTime--) | Ermittelt das Datum und die Uhrzeit der letzten Änderung. |
| [getName()](#getName--) | Gibt den Namen des Eintrags im Archiv zurück. |
| [open()](#open--) | Öffnet den Eintrag zum Extrahieren und stellt einen Stream mit dem Eintragsinhalt bereit. |
| [toString()](#toString--) | Gibt die String‑Repräsentation der Instanz der [CabEntry](../../com.aspose.zip/cabentry)-Klasse zurück. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extrahiert den Eintrag in den bereitgestellten Stream.

Extrahiere einen Eintrag aus einem CAB‑Archiv.

```

``````

try (CabArchive archive = new CabArchive("archive.cab")) {
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

     try (CabArchive archive = new CabArchive("archive.cab")) {
         archive.getEntries().get(0).extract("data.bin");
     }
 
```



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | java.lang.String | Der Pfad zur Zieldatei. Wenn die Datei bereits existiert, wird sie überschrieben. |

**Returns:**
java.io.File – die Dateiinformation einer zusammengesetzten Datei
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


Ermittelt das Datum und die Uhrzeit der letzten Änderung.

**Returns:**
java.util.Date – das zuletzt geänderte Datum und die Uhrzeit.
### getName() {#getName--}
```
public final String getName()
```


Gibt den Namen des Eintrags im Archiv zurück.

**Returns:**
java.lang.String - der Name des Eintrags im Archiv
### open() {#open--}
```
public final InputStream open()
```


Öffnet den Eintrag zum Extrahieren und stellt einen Stream mit dem Eintragsinhalt bereit.

Verwendung:

```

``````

CabArchive archive = new CabArchive("archive.cab");
CabEntry entry = archive.getEntries().get(0);
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


Returns string representation of the instance of the [CabEntry](../../com.aspose.zip/cabentry) class.

**Returns:**
java.lang.String - string representation of this object
