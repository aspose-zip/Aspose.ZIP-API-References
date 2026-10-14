---
title: "PPMdCompressionSettings"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "إعدادات ضغط PPMd داخل أرشيف ZIP."
type: docs
weight: 93
url: /ar/java/com.aspose.zip/ppmdcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class PPMdCompressionSettings extends CompressionSettings
```

إعدادات ضغط PPMd داخل أرشيف ZIP.

PPMd هو خوارزمية ضغط بيانات تم تطويرها بواسطة دميتري شكارين. تعتمد هذه الخوارزمية على مطابقة العبارات التنبؤية في سياقات متعددة الترتيب.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [PPMdCompressionSettings(int modelOrder, int suballocatorSize)](#PPMdCompressionSettings-int-int-) | ينشئ مثيلًا جديدًا من الفئة [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings). |
| [PPMdCompressionSettings()](#PPMdCompressionSettings--) | ينشئ مثيلًا جديدًا من الفئة [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings) مع ترتيب النموذج الافتراضي وحجم المخصص الفرعي. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getModelOrder()](#getModelOrder--) | يحصل على ترتيب النموذج. |
| [getSuballocatorSize()](#getSuballocatorSize--) | يحصل على حجم المخصص الفرعي بالميغابايت. |
### PPMdCompressionSettings(int modelOrder, int suballocatorSize) {#PPMdCompressionSettings-int-int-}
```
public PPMdCompressionSettings(int modelOrder, int suballocatorSize)
```


ينشئ مثيلًا جديدًا من الفئة [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings).

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings(4, 10)))) {
archive.createEntry(\"data.bin\", \"data.bin\");
archive.save("zipFile.zip");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| modelOrder | int | Order of the model.

Bigger model orders almost surely results in better compression and surely more memory and CPU usage. |
| suballocatorSize | int | Memory size in MB suballocator may consume.

The PPMd algorithm might need a lot of memory, especially when used on large files and/or used with large model order. If ppmd needs more memory than you give it, the compression will be worse. |

### PPMdCompressionSettings() {#PPMdCompressionSettings--}
```
public PPMdCompressionSettings()
```


Initializes a new instance of the [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings) class with default model order and sub-allocator size.

```

``````

     try (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings()))) {
         archive.createEntry("data.bin", "data.bin");
         archive.save("zipFile.zip");
     }
 
```

ترتيب النموذج الافتراضي هو 8، وحجم المخصص الفرعي هو 50 ميغابايت.

### getModelOrder() {#getModelOrder--}
```
public final int getModelOrder()
```


يحصل على ترتيب النموذج.

**Returns:**
int - ترتيب النموذج
### getSuballocatorSize() {#getSuballocatorSize--}
```
public final int getSuballocatorSize()
```


يحصل على حجم المخصص الفرعي بالميغابايت.

**Returns:**
int - حجم المخصص الفرعي بالميغابايت
