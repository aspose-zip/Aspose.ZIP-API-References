---
title: "AppleLz4CompressionSettings"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "إعدادات ضغط LZ4 داخل ملف أرشيف Apple .aar"
type: docs
weight: 21
url: /ar/java/com.aspose.zip/applelz4compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings)
```
public class AppleLz4CompressionSettings extends AppleCompressionSettings
```

الإعدادات لضغط LZ4 داخل ملف Apple Archive (.aar).
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [AppleLz4CompressionSettings(int blockSize)](#AppleLz4CompressionSettings-int-) | ينشئ مثلاً جديداً من الفئة [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings). |
| [AppleLz4CompressionSettings()](#AppleLz4CompressionSettings--) | ينشئ مثلاً جديداً من الفئة [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings) مع معلمات افتراضية. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | يحصل على حجم كل كتلة مضغوطة `pbz4`/`bv41`. |
### AppleLz4CompressionSettings(int blockSize) {#AppleLz4CompressionSettings-int-}
```
public AppleLz4CompressionSettings(int blockSize)
```


ينشئ مثلاً جديداً من الفئة [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| blockSize | int | حجم كل كتلة مضغوطة `pbz4`/`bv41`. |

### AppleLz4CompressionSettings() {#AppleLz4CompressionSettings--}
```
public AppleLz4CompressionSettings()
```


ينشئ مثلاً جديداً من الفئة [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings) مع معلمات افتراضية.

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


يحصل على حجم كل كتلة مضغوطة `pbz4`/`bv41`.

القيمة: القيمة الافتراضية هي 4 MiB.

**Returns:**
int - حجم كل كتلة مضغوطة `pbz4`/`bv41`.
