---
title: "Bzip2CompressionSettings"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "إعدادات ضغط Bzip2 داخل أرشيف ZIP."
type: docs
weight: 41
url: /ar/java/com.aspose.zip/bzip2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class Bzip2CompressionSettings extends CompressionSettings
```

إعدادات ضغط Bzip2 داخل أرشيف ZIP.

يقوم bzip2 بضغط الملفات باستخدام خوارزمية ضغط النص بترتيب الكتل Burrows-Wheeler، وترميز هوفمان.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [Bzip2CompressionSettings(int blockSize)](#Bzip2CompressionSettings-int-) | ينشئ مثيلًا جديدًا من الفئة [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings). |
| [Bzip2CompressionSettings()](#Bzip2CompressionSettings--) | ينشئ مثيلًا جديدًا من الفئة [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings) بحجم كتلة افتراضي يساوي 9 مئات من الكيلوبايت. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | حجم الكتلة بالمئات من الكيلوبايت. |
### Bzip2CompressionSettings(int blockSize) {#Bzip2CompressionSettings-int-}
```
public Bzip2CompressionSettings(int blockSize)
```


ينشئ مثيلًا جديدًا من الفئة [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings).

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings(1)))) {
archive.createEntry(\"data.bin\", \"data.bin\");
archive.save(zipFile);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| blockSize | int | Block size in hundreds of kilobytes. |

### Bzip2CompressionSettings() {#Bzip2CompressionSettings--}
```
public Bzip2CompressionSettings()
```


Initializes a new instance of the [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings) class with default block size, equals to 9 hundred of kilobytes.

```

``````

     try (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings()))) {
         archive.createEntry("data.bin", "data.bin");
         archive.save(zipFile);
     }
 
```



### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


حجم الكتلة بالمئات من الكيلوبايت.

**Returns:**
int - حجم الكتلة بالمئات من الكيلوبايت
