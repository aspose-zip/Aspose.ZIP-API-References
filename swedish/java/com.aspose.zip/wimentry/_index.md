---
title: "WimEntry"
second_title: "Aspose.ZIP för Java API-referens"
description: "Representerar en enskild fil eller katalog i wim-avbilden."
type: docs
weight: 132
url: /sv/java/com.aspose.zip/wimentry/
---

**Inheritance:**
java.lang.Object
```
public abstract class WimEntry
```

Representerar en enskild fil eller katalog i wim-avbilden.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getAlternateDataStreams()](#getAlternateDataStreams--) | Hämtar namnen på de alternativa dataströmmarna för filen eller katalogen. |
| [getArchive()](#getArchive--) | Hämtar arkivet som posten tillhör. |
| [getChangeTime()](#getChangeTime--) | Hämtar den senaste gången filen eller katalogen ändrades. |
| [getCreationTime()](#getCreationTime--) | Hämtar skapandetiden för filen eller katalogen. |
| [getFileAttributes()](#getFileAttributes--) | Hämtar filens eller katalogens attribut. |
| [getFullPath()](#getFullPath--) | Hämtar den fullständiga sökvägen för posten i avbilden. |
| [getHardLink()](#getHardLink--) | Hämtar hårdlänks-ID:t för filen eller katalogen. |
| [getImage()](#getImage--) | Hämtar avbilden som posten tillhör. |
| [getLastAccessTime()](#getLastAccessTime--) | Hämtar den senaste åtkomsttiden för filen eller katalogen. |
| [getLastWriteTime()](#getLastWriteTime--) | Hämtar ändringstiden för filen eller katalogen. |
| [getModificationTime()](#getModificationTime--) | Hämtar ändringstiden för filen eller katalogen. |
| [getName()](#getName--) | Hämtar namnet på posten i avbilden. |
| [getParent()](#getParent--) | Hämtar den överordnade katalogen som posten tillhör. |
| [getShortName()](#getShortName--) | Hämtar det korta namnet på posten i avbilden. |
| [hasHardLinks()](#hasHardLinks--) | Hämtar om filen eller katalogen är känd under andra namn. |
| [isDirectory()](#isDirectory--) | Hämtar ett värde som indikerar om posten representerar en katalog. |
| [toString()](#toString--) | Returnerar en strängrepresentation av instansen av klassen [WimEntry](../../com.aspose.zip/wimentry). |
### getAlternateDataStreams() {#getAlternateDataStreams--}
```
public final String[] getAlternateDataStreams()
```


Hämtar namnen på de alternativa dataströmmarna för filen eller katalogen.

**Returns:**
java.lang.String[] - namnen på de alternativa dataströmmarna för filen eller katalogen
### getArchive() {#getArchive--}
```
public final WimArchive getArchive()
```


Hämtar arkivet som posten tillhör.

**Returns:**
[WimArchive](../../com.aspose.zip/wimarchive) - the archive the entry belongs to
### getChangeTime() {#getChangeTime--}
```
public final Date getChangeTime()
```


Hämtar den senaste gången filen eller katalogen ändrades.

**Returns:**
java.util.Date - den senaste tidpunkten filen eller katalogen ändrades
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


Hämtar skapandetiden för filen eller katalogen.

**Returns:**
java.util.Date - skapandetiden för filen eller katalogen
### getFileAttributes() {#getFileAttributes--}
```
public final int getFileAttributes()
```


Hämtar filens eller katalogens attribut.

**Returns:**
int - filens eller katalogens attribut
### getFullPath() {#getFullPath--}
```
public final String getFullPath()
```


Hämtar den fullständiga sökvägen för posten i avbilden.

**Returns:**
java.lang.String - den fullständiga sökvägen för posten i avbilden
### getHardLink() {#getHardLink--}
```
public final long getHardLink()
```


Hämtar hårdlänks-ID:t för filen eller katalogen.

**Returns:**
long - hårdlänks-ID för filen eller katalogen
### getImage() {#getImage--}
```
public final WimImage getImage()
```


Hämtar avbilden som posten tillhör.

**Returns:**
[WimImage](../../com.aspose.zip/wimimage) - the image the entry belongs to
### getLastAccessTime() {#getLastAccessTime--}
```
public final Date getLastAccessTime()
```


Hämtar den senaste åtkomsttiden för filen eller katalogen.

**Returns:**
java.util.Date - den senaste åtkomsttiden för filen eller katalogen
### getLastWriteTime() {#getLastWriteTime--}
```
public final Date getLastWriteTime()
```


Hämtar ändringstiden för filen eller katalogen.

**Returns:**
java.util.Date - modifieringstiden för filen eller katalogen
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Hämtar ändringstiden för filen eller katalogen.

**Returns:**
java.util.Date - modifieringstiden för filen eller katalogen
### getName() {#getName--}
```
public final String getName()
```


Hämtar namnet på posten i avbilden.

**Returns:**
java.lang.String - namnet på posten i avbilden
### getParent() {#getParent--}
```
public final WimDirectoryEntry getParent()
```


Hämtar den överordnade katalogen som posten tillhör.

**Returns:**
[WimDirectoryEntry](../../com.aspose.zip/wimdirectoryentry) - the parent directory the entry belongs to
### getShortName() {#getShortName--}
```
public final String getShortName()
```


Hämtar det korta namnet på posten i avbilden.

**Returns:**
java.lang.String - det korta namnet på posten i avbilden
### hasHardLinks() {#hasHardLinks--}
```
public final boolean hasHardLinks()
```


Hämtar om filen eller katalogen är känd under andra namn.

**Returns:**
boolean - om filen eller katalogen är känd under andra namn
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Hämtar ett värde som indikerar om posten representerar en katalog.

**Returns:**
boolean - ett värde som indikerar om posten representerar en katalog
### toString() {#toString--}
```
public String toString()
```


Returnerar en strängrepresentation av instansen av klassen [WimEntry](../../com.aspose.zip/wimentry).

**Returns:**
java.lang.String - strängrepresentation av detta objekt
