---
title: "IsoEntry"
second_title: "Aspose.ZIP for Java API Referansı"
description: "ISO arşivinde bir giriş dosyasını veya dizinini temsil eder."
type: docs
weight: 72
url: /tr/java/com.aspose.zip/isoentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class IsoEntry implements IArchiveFileEntry
```

ISO arşivi içinde bir giriş (dosya veya dizin) temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Girdiyi sağlanan akıma çıkarır. |
| [extract(String path)](#extract-java.lang.String-) | Girdiyi sağlanan yola göre dosya sistemine çıkarır. |
| [getLength()](#getLength--) | Girişin uzunluğunu alır. |
| [getModificationTime()](#getModificationTime--) | Son değiştirilme tarih ve saatini alır. |
| [getName()](#getName--) | Girişin adını alır. |
| [isDirectory()](#isDirectory--) | Girişin bir dizin olup olmadığını gösteren bir değeri alır. |
| [toString()](#toString--) | Geçerli girişi temsil eden bir dize döndürür. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public void extract(OutputStream destination)
```


Girdiyi sağlanan akıma çıkarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| hedef | java.io.OutputStream | hedef akışı |

### extract(String path) {#extract-java.lang.String-}
```
public File extract(String path)
```


Girdiyi sağlanan yola göre dosya sistemine çıkarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | hedef dosyanın yolu. Dosya zaten mevcutsa, üzerine yazılacaktır |

**Returns:**
java.io.File - çıkarılan veriyi içeren java.io.File örneği
### getLength() {#getLength--}
```
public Long getLength()
```


Girişin uzunluğunu alır.

**Returns:**
java.lang.Long - girişin uzunluğu
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Son değiştirilme tarih ve saatini alır.

**Returns:**
java.util.Date - son değiştirilme tarih ve saati
### getName() {#getName--}
```
public final String getName()
```


Girişin adını alır.

**Returns:**
java.lang.String - girişin adı
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Girişin bir dizin olup olmadığını gösteren bir değeri alır.

**Returns:**
boolean - girişin bir dizin olup olmadığını gösteren değer
### toString() {#toString--}
```
public String toString()
```


Geçerli girişi temsil eden bir dize döndürür.

**Returns:**
java.lang.String - girişin adı
