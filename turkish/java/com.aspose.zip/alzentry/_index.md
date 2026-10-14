---
title: "AlzEntry"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Bir ALZ arşivindeki dosya girişini ve onun meta verilerini temsil eder."
type: docs
weight: 13
url: /tr/java/com.aspose.zip/alzentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class AlzEntry implements IArchiveFileEntry
```

Bir ALZ arşivindeki dosya girişini ve onun meta verilerini temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Girişi yazılabilir bir akıma çıkarır. |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | Girişi isteğe bağlı bir parola kullanarak yazılabilir bir akıma çıkarır. |
| [extract(String path)](#extract-java.lang.String-) | Girişi belirtilen dosyaya çıkarır. |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | Girişi isteğe bağlı bir parola kullanarak belirtilen dosyaya çıkarır. |
| [getCompressedSize()](#getCompressedSize--) | Giriş verisinin sıkıştırılmış boyutunu bayt olarak alır. |
| [getLength()](#getLength--) | Bu girişin sıkıştırılmamış uzunluğunu alır. |
| [getName()](#getName--) | Arşivde depolanan giriş adını alır. |
| [getUncompressedSize()](#getUncompressedSize--) | Giriş verisinin sıkıştırılmamış boyutunu bayt olarak alır. |
| [isDirectory()](#isDirectory--) | Bu girişin bir dizin olup olmadığını alır. |
| [open()](#open--) | Girişi açar ve sıkıştırması çözülmüş veriyi içeren bir akış sağlar. |
| [open(String password)](#open-java.lang.String-) | Girişi açar ve sıkıştırması çözülmüş veriyi içeren bir akış sağlar. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Girişi yazılabilir bir akıma çıkarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| hedef | java.io.OutputStream | hedef akışı |

### extract(OutputStream destination, String password) {#extract-java.io.OutputStream-java.lang.String-}
```
public final void extract(OutputStream destination, String password)
```


Girişi isteğe bağlı bir parola kullanarak yazılabilir bir akıma çıkarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| hedef | java.io.OutputStream | hedef akışı |
| password | java.lang.String | Bu giriş için isteğe bağlı şifre |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Girişi belirtilen dosyaya çıkarır. Mevcut bir dosya üzerine yazılır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | hedef dosya yolu |

**Returns:**
java.io.File - çıkarılan dosya
### extract(String path, String password) {#extract-java.lang.String-java.lang.String-}
```
public final File extract(String path, String password)
```


Girişi isteğe bağlı bir parola kullanarak belirtilen dosyaya çıkarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | hedef dosya yolu |
| password | java.lang.String | Bu giriş için isteğe bağlı şifre |

**Returns:**
java.io.File - çıkarılan dosya
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Giriş verisinin sıkıştırılmış boyutunu bayt olarak alır.

**Returns:**
long - bayt cinsinden sıkıştırılmış boyut
### getLength() {#getLength--}
```
public final Long getLength()
```


Bu girişin sıkıştırılmamış uzunluğunu alır.

**Returns:**
java.lang.Long - bayt cinsinden sıkıştırılmamış uzunluk
### getName() {#getName--}
```
public final String getName()
```


Arşivde depolanan giriş adını alır.

**Returns:**
java.lang.String - giriş adı
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Giriş verisinin sıkıştırılmamış boyutunu bayt olarak alır.

**Returns:**
long - bayt cinsinden sıkıştırılmamış boyut
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Bu girişin bir dizin olup olmadığını alır.

**Returns:**
boolean - dizin girişi için `true`
### open() {#open--}
```
public final InputStream open()
```


Girişi açar ve sıkıştırması çözülmüş veriyi içeren bir akış sağlar.

**Returns:**
java.io.InputStream - sıkıştırması çözülmüş giriş verisini içeren akış
### open(String password) {#open-java.lang.String-}
```
public final InputStream open(String password)
```


Girişi açar ve sıkıştırması çözülmüş veriyi içeren bir akış sağlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| password | java.lang.String | Bu giriş için isteğe bağlı şifre |

**Returns:**
java.io.InputStream - sıkıştırması çözülmüş giriş verisini içeren akış
