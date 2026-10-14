---
title: "XarEntry"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Vertegenwoordigt een enkele vermelding binnen xar-archief."
type: docs
weight: 140
url: /nl/java/com.aspose.zip/xarentry/
---

**Inheritance:**
java.lang.Object
```
public abstract class XarEntry
```

Vertegenwoordigt een enkele vermelding binnen xar-archief.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getCreationTime()](#getCreationTime--) | Haalt de aanmaaktijd van het bestand of de map op. |
| [getFullPath()](#getFullPath--) | Haalt het volledige pad van het item binnen het archief op. |
| [getLastAccessTime()](#getLastAccessTime--) | Haalt de laatste toegangstijd van het bestand of de map op. |
| [getLastWriteTime()](#getLastWriteTime--) | Haalt de wijzigingstijd van het bestand of de map op. |
| [getModificationTime()](#getModificationTime--) | Haalt de wijzigingstijd van het bestand of de map op. |
| [getName()](#getName--) | Haalt de naam van het item binnen het archief op. |
| [getParent()](#getParent--) | Haalt de bovenliggende map op waartoe het item behoort. |
| [isDirectory()](#isDirectory--) | Haalt een waarde op die aangeeft of het item een map vertegenwoordigt. |
| [toString()](#toString--) | Retourneert de tekenreeksrepresentatie van de instantie van de [XarEntry](../../com.aspose.zip/xarentry) klasse. |
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


Haalt de aanmaaktijd van het bestand of de map op.

**Returns:**
java.util.Date - de creatietijd van het bestand of de map
### getFullPath() {#getFullPath--}
```
public final String getFullPath()
```


Haalt het volledige pad van het item binnen het archief op.

**Returns:**
java.lang.String - het volledige pad van het item binnen het archief
### getLastAccessTime() {#getLastAccessTime--}
```
public final Date getLastAccessTime()
```


Haalt de laatste toegangstijd van het bestand of de map op.

**Returns:**
java.util.Date - de laatste toegangstijd van het bestand of de map
### getLastWriteTime() {#getLastWriteTime--}
```
public final Date getLastWriteTime()
```


Haalt de wijzigingstijd van het bestand of de map op.

**Returns:**
java.util.Date - de wijzigingstijd van het bestand of de map
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Haalt de wijzigingstijd van het bestand of de map op.

**Returns:**
java.util.Date - de wijzigingstijd van het bestand of de map
### getName() {#getName--}
```
public final String getName()
```


Haalt de naam van het item binnen het archief op.

**Returns:**
java.lang.String - de naam van het item binnen het archief
### getParent() {#getParent--}
```
public final XarDirectoryEntry getParent()
```


Haalt de bovenliggende map op waartoe het item behoort.

**Returns:**
[XarDirectoryEntry](../../com.aspose.zip/xardirectoryentry) - the parent directory the entry belongs to
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Haalt een waarde op die aangeeft of het item een map vertegenwoordigt.

**Returns:**
boolean - een waarde die aangeeft of de entry een map vertegenwoordigt
### toString() {#toString--}
```
public String toString()
```


Retourneert de tekenreeksrepresentatie van de instantie van de [XarEntry](../../com.aspose.zip/xarentry) klasse.

**Returns:**
java.lang.String - tekenreeksrepresentatie van dit object
