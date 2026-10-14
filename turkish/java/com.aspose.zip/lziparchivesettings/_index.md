---
title: "LzipArchiveSettings"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Sınıf, belirli bir lzip arşivinin ayarlarını içerir."
type: docs
weight: 84
url: /tr/java/com.aspose.zip/lziparchivesettings/
---

**Inheritance:**
java.lang.Object
```
public class LzipArchiveSettings
```

Sınıf, belirli bir lzip arşivinin ayarlarını içerir.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [LzipArchiveSettings(int dictionarySize)](#LzipArchiveSettings-int-) | Belirli bir sözlük boyutuyla [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) sınıfının yeni bir örneğini başlatır. |
| [LzipArchiveSettings(int dictionarySize, int maxMemberSize)](#LzipArchiveSettings-int-int-) | Belirli bir sözlük boyutuyla [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) sınıfının yeni bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getCompressionThreads()](#getCompressionThreads--) | Sıkıştırma iş parçacığı sayısını alır. |
| [getDictionarySize()](#getDictionarySize--) | LZMA sıkıştırması tarafından kullanılan sözlüğün boyutunu alır. |
| [getFastSpeed()](#getFastSpeed--) | LZMA filtresinde sözlük boyutu 1 megabayt olan [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) sınıfının örneğini alır. |
| [getFastestSpeed()](#getFastestSpeed--) | LZMA filtresinde sözlük boyutu 65536 bayt olan [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) sınıfının örneğini alır. |
| [getHighCompression()](#getHighCompression--) | LZMA filtresinde sözlük boyutu 32 megabayt olan [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) sınıfının örneğini alır. |
| [getMaxMemberSize()](#getMaxMemberSize--) | lzip arşivindeki bir üyenin maksimum boyutunu bayt cinsinden alır. |
| [getMaximumCompression()](#getMaximumCompression--) | LZMA filtresinde sözlük boyutu 64 megabayt olan [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) sınıfının örneğini alır. |
| [getNormal()](#getNormal--) | LZMA filtresinde sözlük boyutu 16 megabayt olan [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) sınıfının örneğini alır. |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | Sıkıştırma iş parçacığı sayısını ayarlar. |
### LzipArchiveSettings(int dictionarySize) {#LzipArchiveSettings-int-}
```
public LzipArchiveSettings(int dictionarySize)
```


Belirli bir sözlük boyutuyla [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) sınıfının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dictionarySize | int | LZMA sıkıştırması için sözlük boyutu (bayt) |

### LzipArchiveSettings(int dictionarySize, int maxMemberSize) {#LzipArchiveSettings-int-int-}
```
public LzipArchiveSettings(int dictionarySize, int maxMemberSize)
```


Belirli bir sözlük boyutuyla [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) sınıfının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dictionarySize | int | LZMA sıkıştırması için sözlük boyutu (bayt) |
| maxMemberSize | int | lzip arşivindeki bir üyenin maksimum boyutu bayt cinsinden. Varsayılan değer 60 MB'dir. |

### getCompressionThreads() {#getCompressionThreads--}
```
public final int getCompressionThreads()
```


Sıkıştırma iş parçacığı sayısını alır. Değer 1'den büyükse, çok iş parçacıklı sıkıştırma kullanılacaktır.

**Returns:**
int - sıkıştırma iş parçacığı sayısı
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


LZMA sıkıştırması tarafından kullanılan sözlüğün boyutunu alır.

**Returns:**
int - LZMA sıkıştırması tarafından kullanılan sözlüğün boyutu
### getFastSpeed() {#getFastSpeed--}
```
public static LzipArchiveSettings getFastSpeed()
```


LZMA filtresinde sözlük boyutu 1 megabayt olan [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) sınıfının örneğini alır.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 1 megabyte in LZMA filter
### getFastestSpeed() {#getFastestSpeed--}
```
public static LzipArchiveSettings getFastestSpeed()
```


LZMA filtresinde sözlük boyutu 65536 bayt olan [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) sınıfının örneğini alır.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 65536 bytes in LZMA filter
### getHighCompression() {#getHighCompression--}
```
public static LzipArchiveSettings getHighCompression()
```


LZMA filtresinde sözlük boyutu 32 megabayt olan [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) sınıfının örneğini alır.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 32 megabytes in LZMA filter
### getMaxMemberSize() {#getMaxMemberSize--}
```
public final long getMaxMemberSize()
```


lzip arşivindeki bir üyenin maksimum boyutunu bayt cinsinden alır.

**Returns:**
long - lzip arşivindeki bir üyenin maksimum boyutu bayt cinsinden
### getMaximumCompression() {#getMaximumCompression--}
```
public static LzipArchiveSettings getMaximumCompression()
```


LZMA filtresinde sözlük boyutu 64 megabayt olan [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) sınıfının örneğini alır.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 64 megabytes in LZMA filter
### getNormal() {#getNormal--}
```
public static LzipArchiveSettings getNormal()
```


LZMA filtresinde sözlük boyutu 16 megabayt olan [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) sınıfının örneğini alır.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 16 megabytes in LZMA filter
### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


Sıkıştırma iş parçacığı sayısını ayarlar. Değer 1'den büyükse, çok iş parçacıklı sıkıştırma kullanılacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | sıkıştırma iş parçacığı sayısı |

