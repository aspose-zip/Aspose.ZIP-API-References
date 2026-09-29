---
title: "SevenZipBZip2CompressionSettings"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "إعدادات طريقة ضغط BZip2 داخل أرشيف 7z."
type: docs
weight: 109
url: /ar/java/com.aspose.zip/sevenzipbzip2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public class SevenZipBZip2CompressionSettings extends SevenZipCompressionSettings
```

إعدادات طريقة ضغط BZip2 داخل أرشيف 7z.

يقوم Bzip2 بضغط الملفات باستخدام خوارزمية ضغط النص بترتيب الكتل Burrows-Wheeler، وترميز هوفمان.

انظر المزيد: [Bzip2][]


[Bzip2]: https://en.wikipedia.org/wiki/Bzip2
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [SevenZipBZip2CompressionSettings(int blockSize)](#SevenZipBZip2CompressionSettings-int-) | ينشئ مثيلًا جديدًا من الفئة [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings). |
| [SevenZipBZip2CompressionSettings()](#SevenZipBZip2CompressionSettings--) | ينشئ مثيلًا جديدًا من الفئة [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings) بحجم كتلة افتراضي يساوي 9 مئات كيلوبايت. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | حجم الكتلة بالمئات من الكيلوبايت. |
| [getMethod()](#getMethod--) | يحصل على طريقة الضغط أو الفك. |
### SevenZipBZip2CompressionSettings(int blockSize) {#SevenZipBZip2CompressionSettings-int-}
```
public SevenZipBZip2CompressionSettings(int blockSize)
```


ينشئ مثيلًا جديدًا من الفئة [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| blockSize | int | حجم الكتلة بالمئات من الكيلوبايت |

### SevenZipBZip2CompressionSettings() {#SevenZipBZip2CompressionSettings--}
```
public SevenZipBZip2CompressionSettings()
```


ينشئ مثيلًا جديدًا من الفئة [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings) بحجم كتلة افتراضي يساوي 9 مئات كيلوبايت.

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


حجم الكتلة بالمئات من الكيلوبايت.

**Returns:**
int - حجم الكتلة بالمئات من الكيلوبايت
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


يحصل على طريقة الضغط أو الفك.

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method
