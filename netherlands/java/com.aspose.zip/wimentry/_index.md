---
title: "WimEntry"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Vertegenwoordigt een enkel bestand of map binnen wim-image."
type: docs
weight: 132
url: /nl/java/com.aspose.zip/wimentry/
---

**Inheritance:**
java.lang.Object
```
public abstract class WimEntry
```

Vertegenwoordigt een enkel bestand of map binnen wim-image.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getAlternateDataStreams()](#getAlternateDataStreams--) | Haalt de namen van de alternatieve gegevensstromen voor het bestand of de map op. |
| [getArchive()](#getArchive--) | Haalt het archief op waartoe het item behoort. |
| [getChangeTime()](#getChangeTime--) | Haalt de laatste wijzigingstijd van het bestand of de map op. |
| [getCreationTime()](#getCreationTime--) | Haalt de aanmaaktijd van het bestand of de map op. |
| [getFileAttributes()](#getFileAttributes--) | Haalt de attributen van het bestand of de map op. |
| [getFullPath()](#getFullPath--) | Haalt het volledige pad van het item binnen het image op. |
| [getHardLink()](#getHardLink--) | Haalt de hardlink-id van het bestand of de map op. |
| [getImage()](#getImage--) | Haalt het image op waartoe het item behoort. |
| [getLastAccessTime()](#getLastAccessTime--) | Haalt de laatste toegangstijd van het bestand of de map op. |
| [getLastWriteTime()](#getLastWriteTime--) | Haalt de wijzigingstijd van het bestand of de map op. |
| [getModificationTime()](#getModificationTime--) | Haalt de wijzigingstijd van het bestand of de map op. |
| [getName()](#getName--) | Haalt de naam van het item binnen het image op. |
| [getParent()](#getParent--) | Haalt de bovenliggende map op waartoe het item behoort. |
| [getShortName()](#getShortName--) | Haalt de korte naam van het item binnen het image op. |
| [hasHardLinks()](#hasHardLinks--) | Haalt op of het bestand of de map onder andere namen bekend is. |
| [isDirectory()](#isDirectory--) | Haalt een waarde op die aangeeft of het item een map vertegenwoordigt. |
| [toString()](#toString--) | Retourneert de tekenreeksrepresentatie van de instantie van de [WimEntry](../../com.aspose.zip/wimentry) klasse. |
### getAlternateDataStreams() {#getAlternateDataStreams--}
```
public final String[] getAlternateDataStreams()
```


Haalt de namen van de alternatieve gegevensstromen voor het bestand of de map op.

**Returns:**
java.lang.String[] - de namen van de alternatieve gegevensstromen voor het bestand of de map
### getArchive() {#getArchive--}
```
public final WimArchive getArchive()
```


Haalt het archief op waartoe het item behoort.

**Returns:**
[WimArchive](../../com.aspose.zip/wimarchive) - the archive the entry belongs to
### getChangeTime() {#getChangeTime--}
```
public final Date getChangeTime()
```


Haalt de laatste wijzigingstijd van het bestand of de map op.

**Returns:**
java.util.Date - de laatste keer dat het bestand of de map werd gewijzigd
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


Haalt de aanmaaktijd van het bestand of de map op.

**Returns:**
java.util.Date - de creatietijd van het bestand of de map
### getFileAttributes() {#getFileAttributes--}
```
public final int getFileAttributes()
```


Haalt de attributen van het bestand of de map op.

**Returns:**
int - de attributen van het bestand of de map
### getFullPath() {#getFullPath--}
```
public final String getFullPath()
```


Haalt het volledige pad van het item binnen het image op.

**Returns:**
java.lang.String - het volledige pad van het item binnen de image
### getHardLink() {#getHardLink--}
```
public final long getHardLink()
```


Haalt de hardlink-id van het bestand of de map op.

**Returns:**
long - de hardlink‑ID van het bestand of de map
### getImage() {#getImage--}
```
public final WimImage getImage()
```


Haalt het image op waartoe het item behoort.

**Returns:**
[WimImage](../../com.aspose.zip/wimimage) - the image the entry belongs to
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


Haalt de naam van het item binnen het image op.

**Returns:**
java.lang.String - de naam van het item binnen de image
### getParent() {#getParent--}
```
public final WimDirectoryEntry getParent()
```


Haalt de bovenliggende map op waartoe het item behoort.

**Returns:**
[WimDirectoryEntry](../../com.aspose.zip/wimdirectoryentry) - the parent directory the entry belongs to
### getShortName() {#getShortName--}
```
public final String getShortName()
```


Haalt de korte naam van het item binnen het image op.

**Returns:**
java.lang.String - de korte naam van het item binnen de image
### hasHardLinks() {#hasHardLinks--}
```
public final boolean hasHardLinks()
```


Haalt op of het bestand of de map onder andere namen bekend is.

**Returns:**
boolean - of het bestand of de map onder andere namen bekend is
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


Retourneert de tekenreeksrepresentatie van de instantie van de [WimEntry](../../com.aspose.zip/wimentry) klasse.

**Returns:**
java.lang.String - tekenreeksrepresentatie van dit object
