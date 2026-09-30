---
title: "XarEntry"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Xar arşivindeki tek bir girişi temsil eder."
type: docs
weight: 140
url: /tr/java/com.aspose.zip/xarentry/
---

**Inheritance:**
java.lang.Object
```
public abstract class XarEntry
```

Xar arşivindeki tek bir girişi temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getCreationTime()](#getCreationTime--) | Dosya veya dizinin oluşturulma zamanını alır. |
| [getFullPath()](#getFullPath--) | Arşiv içindeki girdinin tam yolunu alır. |
| [getLastAccessTime()](#getLastAccessTime--) | Dosya veya dizinin son erişim zamanını alır. |
| [getLastWriteTime()](#getLastWriteTime--) | Dosyanın veya dizinin değiştirilme zamanını alır. |
| [getModificationTime()](#getModificationTime--) | Dosyanın veya dizinin değiştirilme zamanını alır. |
| [getName()](#getName--) | Arşiv içindeki girdinin adını alır. |
| [getParent()](#getParent--) | Girdinin ait olduğu üst dizini alır. |
| [isDirectory()](#isDirectory--) | Girdinin bir dizin olup olmadığını gösteren değeri alır. |
| [toString()](#toString--) | Bu sınıfın bir örneği olan [XarEntry](../../com.aspose.zip/xarentry) nesnesinin dize temsilini döndürür. |
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


Dosya veya dizinin oluşturulma zamanını alır.

**Returns:**
java.util.Date - dosya veya dizinin oluşturulma zamanı
### getFullPath() {#getFullPath--}
```
public final String getFullPath()
```


Arşiv içindeki girdinin tam yolunu alır.

**Returns:**
java.lang.String - arşiv içindeki girdinin tam yolu
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


Arşiv içindeki girdinin adını alır.

**Returns:**
java.lang.String - arşiv içindeki girdinin adı
### getParent() {#getParent--}
```
public final XarDirectoryEntry getParent()
```


Girdinin ait olduğu üst dizini alır.

**Returns:**
[XarDirectoryEntry](../../com.aspose.zip/xardirectoryentry) - the parent directory the entry belongs to
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


Bu sınıfın bir örneği olan [XarEntry](../../com.aspose.zip/xarentry) nesnesinin dize temsilini döndürür.

**Returns:**
java.lang.String - bu nesnenin dize temsili
