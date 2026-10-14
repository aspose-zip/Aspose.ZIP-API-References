---
title: "AlzEntry"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Stelt een bestandsvermelding in een ALZ-archief voor, samen met de metadata."
type: docs
weight: 13
url: /nl/java/com.aspose.zip/alzentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class AlzEntry implements IArchiveFileEntry
```

Stelt een bestandsvermelding in een ALZ-archief voor, samen met de metadata.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extraheert het item naar een beschrijfbare stroom. |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | Extraheert het item naar een beschrijfbare stroom met een optioneel wachtwoord. |
| [extract(String path)](#extract-java.lang.String-) | Extraheert het item naar het opgegeven bestand. |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | Extraheert het item naar het opgegeven bestand met een optioneel wachtwoord. |
| [getCompressedSize()](#getCompressedSize--) | Haalt de gecomprimeerde grootte van de itemgegevens op in bytes. |
| [getLength()](#getLength--) | Haalt de gedecomprimeerde lengte van dit item op. |
| [getName()](#getName--) | Haalt de naam van het item op die in het archief is opgeslagen. |
| [getUncompressedSize()](#getUncompressedSize--) | Haalt de gedecomprimeerde grootte van de itemgegevens op in bytes. |
| [isDirectory()](#isDirectory--) | Haalt op of dit item een map vertegenwoordigt. |
| [open()](#open--) | Opent het item en levert een stroom met gedecomprimeerde gegevens. |
| [open(String password)](#open-java.lang.String-) | Opent het item en levert een stroom met gedecomprimeerde gegevens. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extraheert het item naar een beschrijfbare stroom.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| bestemming | java.io.OutputStream | bestemmingsstroom |

### extract(OutputStream destination, String password) {#extract-java.io.OutputStream-java.lang.String-}
```
public final void extract(OutputStream destination, String password)
```


Extraheert het item naar een beschrijfbare stroom met een optioneel wachtwoord.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| bestemming | java.io.OutputStream | bestemmingsstroom |
| password | java.lang.String | optioneel wachtwoord voor dit item |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extraheert het item naar het opgegeven bestand. Een bestaand bestand wordt overschreven.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | doelbestandspad |

**Returns:**
java.io.File - geëxtraheerd bestand
### extract(String path, String password) {#extract-java.lang.String-java.lang.String-}
```
public final File extract(String path, String password)
```


Extraheert het item naar het opgegeven bestand met een optioneel wachtwoord.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | doelbestandspad |
| password | java.lang.String | optioneel wachtwoord voor dit item |

**Returns:**
java.io.File - geëxtraheerd bestand
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Haalt de gecomprimeerde grootte van de itemgegevens op in bytes.

**Returns:**
long - gecomprimeerde grootte in bytes
### getLength() {#getLength--}
```
public final Long getLength()
```


Haalt de gedecomprimeerde lengte van dit item op.

**Returns:**
java.lang.Long - ongecomprimeerde lengte in bytes
### getName() {#getName--}
```
public final String getName()
```


Haalt de naam van het item op die in het archief is opgeslagen.

**Returns:**
java.lang.String - naam van invoer
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Haalt de gedecomprimeerde grootte van de itemgegevens op in bytes.

**Returns:**
long - ongecomprimeerde grootte in bytes
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Haalt op of dit item een map vertegenwoordigt.

**Returns:**
boolean - `true` voor een mapinvoer
### open() {#open--}
```
public final InputStream open()
```


Opent het item en levert een stroom met gedecomprimeerde gegevens.

**Returns:**
java.io.InputStream - stream met gedecomprimeerde invoergegevens
### open(String password) {#open-java.lang.String-}
```
public final InputStream open(String password)
```


Opent het item en levert een stroom met gedecomprimeerde gegevens.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| password | java.lang.String | optioneel wachtwoord voor dit item |

**Returns:**
java.io.InputStream - stream met gedecomprimeerde invoergegevens
