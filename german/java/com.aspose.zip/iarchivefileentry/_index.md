---
title: "IArchiveFileEntry"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Dieses Interface stellt einen Eintrag einer Archivdatei dar."
type: docs
weight: 162
url: /de/java/com.aspose.zip/iarchivefileentry/
---
```
public interface IArchiveFileEntry
```

Dieses Interface stellt einen Eintrag einer Archivdatei dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrahiert den Eintrag in den bereitgestellten Stream. |
| [extract(String path)](#extract-java.lang.String-) | Extrahiert den Eintrag in das Dateisystem über den angegebenen Pfad. |
| [getLength()](#getLength--) | Gibt die Länge des Eintrags in Bytes zurück. |
| [getName()](#getName--) | Ermittelt den Namen des Eintrags. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public abstract void extract(OutputStream destination)
```


Extrahiert den Eintrag in den bereitgestellten Stream.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Ziel | java.io.OutputStream | Ziel-Stream. Muss beschreibbar sein. |

### extract(String path) {#extract-java.lang.String-}
```
public abstract File extract(String path)
```


Extrahiert den Eintrag in das Dateisystem über den angegebenen Pfad.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | java.lang.String | Der Pfad zur Zieldatei. Wenn die Datei bereits existiert, wird sie überschrieben. |

**Returns:**
java.io.File - java.io.File-Instanz, die extrahierte Daten enthält
### getLength() {#getLength--}
```
public abstract Long getLength()
```


Gibt die Länge des Eintrags in Bytes zurück.

**Returns:**
java.lang.Long – die Länge des Eintrags in Bytes
### getName() {#getName--}
```
public abstract String getName()
```


Ermittelt den Namen des Eintrags.

Archive nur zur Kompression, wie gzip, bzip2, lzip, lzma, xz, z, haben den Namen \"File.bin\", sofern kein anderer Name in den Headern gefunden wird.

**Returns:**
java.lang.String - der Name des Eintrags
