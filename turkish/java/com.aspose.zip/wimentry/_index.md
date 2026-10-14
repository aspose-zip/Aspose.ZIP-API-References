---
title: "WimEntry"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Wim görüntüsündeki tek bir dosya veya dizini temsil eder."
type: docs
weight: 132
url: /tr/java/com.aspose.zip/wimentry/
---

**Inheritance:**
java.lang.Object
```
public abstract class WimEntry
```

Wim görüntüsündeki tek bir dosya veya dizini temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getAlternateDataStreams()](#getAlternateDataStreams--) | Dosya veya dizin için alternatif veri akışlarının adlarını alır. |
| [getArchive()](#getArchive--) | Girdinin ait olduğu arşivi alır. |
| [getChangeTime()](#getChangeTime--) | Dosya veya dizinin son değişiklik zamanını alır. |
| [getCreationTime()](#getCreationTime--) | Dosya veya dizinin oluşturulma zamanını alır. |
| [getFileAttributes()](#getFileAttributes--) | Dosya veya dizin özniteliklerini alır. |
| [getFullPath()](#getFullPath--) | Görüntü içindeki girişin tam yolunu alır. |
| [getHardLink()](#getHardLink--) | Dosya veya dizinin hardlink kimliğini alır. |
| [getImage()](#getImage--) | Girişin ait olduğu görüntüyü alır. |
| [getLastAccessTime()](#getLastAccessTime--) | Dosya veya dizinin son erişim zamanını alır. |
| [getLastWriteTime()](#getLastWriteTime--) | Dosyanın veya dizinin değiştirilme zamanını alır. |
| [getModificationTime()](#getModificationTime--) | Dosyanın veya dizinin değiştirilme zamanını alır. |
| [getName()](#getName--) | Görüntü içindeki girdinin adını alır. |
| [getParent()](#getParent--) | Girdinin ait olduğu üst dizini alır. |
| [getShortName()](#getShortName--) | Görüntü içindeki girdinin kısa adını alır. |
| [hasHardLinks()](#hasHardLinks--) | Dosyanın veya dizinin başka adlarla bilinip bilinmediğini alır. |
| [isDirectory()](#isDirectory--) | Girdinin bir dizin olup olmadığını gösteren değeri alır. |
| [toString()](#toString--) | [WimEntry](../../com.aspose.zip/wimentry) sınıfının örneğinin dize temsilini döndürür. |
### getAlternateDataStreams() {#getAlternateDataStreams--}
```
public final String[] getAlternateDataStreams()
```


Dosya veya dizin için alternatif veri akışlarının adlarını alır.

**Returns:**
java.lang.String[] - dosya veya dizin için alternatif veri akışlarının adları
### getArchive() {#getArchive--}
```
public final WimArchive getArchive()
```


Girdinin ait olduğu arşivi alır.

**Returns:**
[WimArchive](../../com.aspose.zip/wimarchive) - the archive the entry belongs to
### getChangeTime() {#getChangeTime--}
```
public final Date getChangeTime()
```


Dosya veya dizinin son değişiklik zamanını alır.

**Returns:**
java.util.Date - dosya veya dizinin en son değiştirildiği zaman
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


Dosya veya dizinin oluşturulma zamanını alır.

**Returns:**
java.util.Date - dosya veya dizinin oluşturulma zamanı
### getFileAttributes() {#getFileAttributes--}
```
public final int getFileAttributes()
```


Dosya veya dizin özniteliklerini alır.

**Returns:**
int - dosya veya dizin öznitelikleri
### getFullPath() {#getFullPath--}
```
public final String getFullPath()
```


Görüntü içindeki girişin tam yolunu alır.

**Returns:**
java.lang.String - görüntü içindeki girdinin tam yolu
### getHardLink() {#getHardLink--}
```
public final long getHardLink()
```


Dosya veya dizinin hardlink kimliğini alır.

**Returns:**
long - dosya veya dizinin hardlink kimliği
### getImage() {#getImage--}
```
public final WimImage getImage()
```


Girişin ait olduğu görüntüyü alır.

**Returns:**
[WimImage](../../com.aspose.zip/wimimage) - the image the entry belongs to
### getLastAccessTime() {#getLastAccessTime--}
```
public final Date getLastAccessTime()
```


Dosya veya dizinin son erişim zamanını alır.

**Returns:**
java.util.Date - dosya veya dizinin son erişim zamanı
### getLastWriteTime() {#getLastWriteTime--}
```
public final Date getLastWriteTime()
```


Dosyanın veya dizinin değiştirilme zamanını alır.

**Returns:**
java.util.Date - dosya veya dizinin değiştirilme zamanı
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Dosyanın veya dizinin değiştirilme zamanını alır.

**Returns:**
java.util.Date - dosya veya dizinin değiştirilme zamanı
### getName() {#getName--}
```
public final String getName()
```


Görüntü içindeki girdinin adını alır.

**Returns:**
java.lang.String - görüntü içindeki girdinin adı
### getParent() {#getParent--}
```
public final WimDirectoryEntry getParent()
```


Girdinin ait olduğu üst dizini alır.

**Returns:**
[WimDirectoryEntry](../../com.aspose.zip/wimdirectoryentry) - the parent directory the entry belongs to
### getShortName() {#getShortName--}
```
public final String getShortName()
```


Görüntü içindeki girdinin kısa adını alır.

**Returns:**
java.lang.String - görüntü içindeki girdinin kısa adı
### hasHardLinks() {#hasHardLinks--}
```
public final boolean hasHardLinks()
```


Dosyanın veya dizinin başka adlarla bilinip bilinmediğini alır.

**Returns:**
boolean - dosya veya dizinin başka adlarla bilinip bilinmediği
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Girdinin bir dizin olup olmadığını gösteren değeri alır.

**Returns:**
boolean - girişin bir dizin olup olmadığını gösteren değer
### toString() {#toString--}
```
public String toString()
```


[WimEntry](../../com.aspose.zip/wimentry) sınıfının örneğinin dize temsilini döndürür.

**Returns:**
java.lang.String - bu nesnenin dize temsili
