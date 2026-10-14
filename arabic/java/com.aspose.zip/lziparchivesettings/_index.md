---
title: "LzipArchiveSettings"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "الفئة تحتوي على إعداد أرشيف lzip معين."
type: docs
weight: 84
url: /ar/java/com.aspose.zip/lziparchivesettings/
---

**Inheritance:**
java.lang.Object
```
public class LzipArchiveSettings
```

الفئة تحتوي على إعداد أرشيف lzip معين.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [LzipArchiveSettings(int dictionarySize)](#LzipArchiveSettings-int-) | ينشئ مثيلاً جديداً من [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) بحجم قاموس معين. |
| [LzipArchiveSettings(int dictionarySize, int maxMemberSize)](#LzipArchiveSettings-int-int-) | ينشئ مثيلاً جديداً من [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) بحجم قاموس معين. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getCompressionThreads()](#getCompressionThreads--) | يحصل على عدد خيوط الضغط. |
| [getDictionarySize()](#getDictionarySize--) | يحصل على حجم القاموس المستخدم في ضغط LZMA. |
| [getFastSpeed()](#getFastSpeed--) | يحصل على مثيل فئة [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) بحجم قاموس يساوي 1 ميغابايت في مرشح LZMA. |
| [getFastestSpeed()](#getFastestSpeed--) | يحصل على مثيل فئة [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) بحجم قاموس يساوي 65536 بايت في مرشح LZMA. |
| [getHighCompression()](#getHighCompression--) | يحصل على مثيل فئة [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) بحجم قاموس يساوي 32 ميغابايت في مرشح LZMA. |
| [getMaxMemberSize()](#getMaxMemberSize--) | يحصل على الحد الأقصى لحجم عضو واحد في أرشيف lzip معروضًا بالبايت. |
| [getMaximumCompression()](#getMaximumCompression--) | يحصل على مثيل فئة [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) بحجم قاموس يساوي 64 ميغابايت في مرشح LZMA. |
| [getNormal()](#getNormal--) | يحصل على مثيل فئة [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) بحجم قاموس يساوي 16 ميغابايت في مرشح LZMA. |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | يضبط عدد خيوط الضغط. |
### LzipArchiveSettings(int dictionarySize) {#LzipArchiveSettings-int-}
```
public LzipArchiveSettings(int dictionarySize)
```


ينشئ مثيلاً جديداً من [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) بحجم قاموس معين.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| dictionarySize | int | حجم القاموس لضغط LZMA بالبايت |

### LzipArchiveSettings(int dictionarySize, int maxMemberSize) {#LzipArchiveSettings-int-int-}
```
public LzipArchiveSettings(int dictionarySize, int maxMemberSize)
```


ينشئ مثيلاً جديداً من [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) بحجم قاموس معين.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| dictionarySize | int | حجم القاموس لضغط LZMA بالبايت |
| maxMemberSize | int | الحد الأقصى لحجم عضو واحد في أرشيف lzip معروض بالبايت. القيمة الافتراضية هي 60 ميغابايت. |

### getCompressionThreads() {#getCompressionThreads--}
```
public final int getCompressionThreads()
```


يحصل على عدد خيوط الضغط. إذا كانت القيمة أكبر من 1، سيتم استخدام ضغط متعدد الخيوط.

**Returns:**
int - عدد خيوط الضغط
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


يحصل على حجم القاموس المستخدم في ضغط LZMA.

**Returns:**
int - حجم القاموس المستخدم في ضغط LZMA
### getFastSpeed() {#getFastSpeed--}
```
public static LzipArchiveSettings getFastSpeed()
```


يحصل على مثيل فئة [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) بحجم قاموس يساوي 1 ميغابايت في مرشح LZMA.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 1 megabyte in LZMA filter
### getFastestSpeed() {#getFastestSpeed--}
```
public static LzipArchiveSettings getFastestSpeed()
```


يحصل على مثيل فئة [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) بحجم قاموس يساوي 65536 بايت في مرشح LZMA.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 65536 bytes in LZMA filter
### getHighCompression() {#getHighCompression--}
```
public static LzipArchiveSettings getHighCompression()
```


يحصل على مثيل فئة [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) بحجم قاموس يساوي 32 ميغابايت في مرشح LZMA.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 32 megabytes in LZMA filter
### getMaxMemberSize() {#getMaxMemberSize--}
```
public final long getMaxMemberSize()
```


يحصل على الحد الأقصى لحجم عضو واحد في أرشيف lzip معروضًا بالبايت.

**Returns:**
long - الحد الأقصى لحجم عضو واحد في أرشيف lzip معروض بالبايت
### getMaximumCompression() {#getMaximumCompression--}
```
public static LzipArchiveSettings getMaximumCompression()
```


يحصل على مثيل فئة [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) بحجم قاموس يساوي 64 ميغابايت في مرشح LZMA.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 64 megabytes in LZMA filter
### getNormal() {#getNormal--}
```
public static LzipArchiveSettings getNormal()
```


يحصل على مثيل فئة [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) بحجم قاموس يساوي 16 ميغابايت في مرشح LZMA.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 16 megabytes in LZMA filter
### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


يضبط عدد خيوط الضغط. إذا كانت القيمة أكبر من 1، سيتم استخدام الضغط متعدد الخيوط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| قيمة | int | عدد خيوط الضغط |

