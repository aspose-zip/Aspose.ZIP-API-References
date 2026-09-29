---
title: "XarBzip2CompressionSettings"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "إعدادات طريقة ضغط Bzip2."
type: docs
weight: 137
url: /ar/java/com.aspose.zip/xarbzip2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings)
```
public class XarBzip2CompressionSettings extends XarCompressionSettings
```

إعدادات طريقة ضغط Bzip2.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [XarBzip2CompressionSettings(int blockSize)](#XarBzip2CompressionSettings-int-) | ينشئ مثيلاً جديداً من الفئة [XarBzip2CompressionSettings](../../com.aspose.zip/xarbzip2compressionsettings). |
| [XarBzip2CompressionSettings()](#XarBzip2CompressionSettings--) | ينشئ مثيلاً جديداً من الفئة [XarBzip2CompressionSettings](../../com.aspose.zip/xarbzip2compressionsettings) بحجم كتلة افتراضي يساوي 9 مئات من الكيلوبايت. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | حجم الكتلة بالمئات من الكيلوبايت. |
### XarBzip2CompressionSettings(int blockSize) {#XarBzip2CompressionSettings-int-}
```
public XarBzip2CompressionSettings(int blockSize)
```


ينشئ مثيلاً جديداً من الفئة [XarBzip2CompressionSettings](../../com.aspose.zip/xarbzip2compressionsettings).

```

``````

try (XarArchive archive = new XarArchive()) {
archive.createEntry("data.bin", "data.bin", false, new XarBzip2CompressionSettings(1));
archive.save("archive.xar");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| blockSize | int | block size in hundreds of kilobytes |

### XarBzip2CompressionSettings() {#XarBzip2CompressionSettings--}
```
public XarBzip2CompressionSettings()
```


Initializes a new instance of the [XarBzip2CompressionSettings](../../com.aspose.zip/xarbzip2compressionsettings) class with default block size, equals to 9 hundred of kilobytes.

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


Block size in hundreds of kilobytes.

**Returns:**
int - block size in hundreds of kilobytes
