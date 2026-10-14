---
title: "AppleLzmaCompressionSettings"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "إعدادات ضغط LZMA داخل ملف Apple Archive بامتداد .aar."
type: docs
weight: 23
url: /ar/java/com.aspose.zip/applelzmacompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings)
```
public class AppleLzmaCompressionSettings extends AppleCompressionSettings
```

الإعدادات لضغط LZMA داخل ملف Apple Archive (.aar).
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [AppleLzmaCompressionSettings(int blockSize)](#AppleLzmaCompressionSettings-int-) | يُنشئ مثيلًا جديدًا من الفئة [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings). |
| [AppleLzmaCompressionSettings(int blockSize, int dictionarySize)](#AppleLzmaCompressionSettings-int-int-) | يُنشئ مثيلًا جديدًا من الفئة [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings). |
| [AppleLzmaCompressionSettings(int blockSize, int dictionarySize, int fastBytes)](#AppleLzmaCompressionSettings-int-int-int-) | يُنشئ مثيلًا جديدًا من الفئة [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings). |
| [AppleLzmaCompressionSettings()](#AppleLzmaCompressionSettings--) | يُنشئ مثيلًا جديدًا من الفئة [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) مع المعلمات الافتراضية. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | يحصل على حجم كل كتلة بيانات قبل الضغط. |
| [getDictionarySize()](#getDictionarySize--) | يحصل على حجم القاموس المستخدم للضغط. |
| [getFastBytes()](#getFastBytes--) | يحصل على عدد البايتات السريعة المستخدمة للضغط. |
### AppleLzmaCompressionSettings(int blockSize) {#AppleLzmaCompressionSettings-int-}
```
public AppleLzmaCompressionSettings(int blockSize)
```


يُنشئ مثيلًا جديدًا من الفئة [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| blockSize | int | حجم كل كتلة بيانات قبل الضغط. |

### AppleLzmaCompressionSettings(int blockSize, int dictionarySize) {#AppleLzmaCompressionSettings-int-int-}
```
public AppleLzmaCompressionSettings(int blockSize, int dictionarySize)
```


يُنشئ مثيلًا جديدًا من الفئة [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| blockSize | int | حجم كل كتلة بيانات قبل الضغط. |
| dictionarySize | int | حجم القاموس المستخدم للضغط. |

### AppleLzmaCompressionSettings(int blockSize, int dictionarySize, int fastBytes) {#AppleLzmaCompressionSettings-int-int-int-}
```
public AppleLzmaCompressionSettings(int blockSize, int dictionarySize, int fastBytes)
```


يُنشئ مثيلًا جديدًا من الفئة [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| blockSize | int | حجم كل كتلة بيانات قبل الضغط. |
| dictionarySize | int | حجم القاموس المستخدم للضغط. |
| fastBytes | int | عدد البايتات السريعة المستخدمة للضغط. |

### AppleLzmaCompressionSettings() {#AppleLzmaCompressionSettings--}
```
public AppleLzmaCompressionSettings()
```


يُنشئ مثيلًا جديدًا من الفئة [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) مع المعلمات الافتراضية.

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


يحصل على حجم كل كتلة بيانات قبل الضغط.

القيمة: القيمة الافتراضية هي 4 MiB.

**Returns:**
int - حجم كل كتلة بيانات قبل الضغط.
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


يحصل على حجم القاموس المستخدم للضغط.

القيمة: القيمة الافتراضية هي 8 ميغابايت.

**Returns:**
int - حجم القاموس المستخدم للضغط.
### getFastBytes() {#getFastBytes--}
```
public final int getFastBytes()
```


يحصل على عدد البايتات السريعة المستخدمة للضغط.

القيمة: القيمة الافتراضية هي 32.

**Returns:**
int - عدد البايتات السريعة المستخدمة للضغط.
