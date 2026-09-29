---
title: "IsoEntry"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Stelt een bestand of map binnen een ISO-archief voor."
type: docs
weight: 72
url: /nl/java/com.aspose.zip/isoentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class IsoEntry implements IArchiveFileEntry
```

Vertegenwoordigt een invoer (bestand of map) binnen een ISO-archief.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extraheert het item naar de opgegeven stream. |
| [extract(String path)](#extract-java.lang.String-) | Extraheert het item naar het bestandssysteem via het opgegeven pad. |
| [getLength()](#getLength--) | Haalt de lengte van het item op. |
| [getModificationTime()](#getModificationTime--) | Haalt de datum en tijd van de laatste wijziging op. |
| [getName()](#getName--) | Haalt de naam van het item op. |
| [isDirectory()](#isDirectory--) | Haalt een waarde op die aangeeft of het item een map is. |
| [toString()](#toString--) | Retourneert een string die de huidige invoer weergeeft. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public void extract(OutputStream destination)
```


Extraheert het item naar de opgegeven stream.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| bestemming | java.io.OutputStream | bestemmingsstroom |

### extract(String path) {#extract-java.lang.String-}
```
public File extract(String path)
```


Extraheert het item naar het bestandssysteem via het opgegeven pad.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | het pad naar het bestemmingsbestand. Als het bestand al bestaat, wordt het overschreven |

**Returns:**
java.io.File - java.io.File‑instantie die geëxtraheerde gegevens bevat
### getLength() {#getLength--}
```
public Long getLength()
```


Haalt de lengte van het item op.

**Returns:**
java.lang.Long - de lengte van de entry
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Haalt de datum en tijd van de laatste wijziging op.

**Returns:**
java.util.Date - datum en tijd van laatste wijziging
### getName() {#getName--}
```
public final String getName()
```


Haalt de naam van het item op.

**Returns:**
java.lang.String - de naam van de entry
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Haalt een waarde op die aangeeft of het item een map is.

**Returns:**
boolean - een waarde die aangeeft of de entry een map vertegenwoordigt
### toString() {#toString--}
```
public String toString()
```


Retourneert een string die de huidige invoer weergeeft.

**Returns:**
java.lang.String - de naam van de entry
