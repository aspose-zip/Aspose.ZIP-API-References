---
title: "SevenZipPPMdCompressionSettings"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "إعدادات طريقة ضغط PPMd داخل أرشيف 7z."
type: docs
weight: 117
url: /ar/java/com.aspose.zip/sevenzipppmdcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public final class SevenZipPPMdCompressionSettings extends SevenZipCompressionSettings
```

إعدادات طريقة ضغط PPMd داخل أرشيف 7z.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [SevenZipPPMdCompressionSettings(int maxOrder, int suballocatorSize)](#SevenZipPPMdCompressionSettings-int-int-) | ينشئ إعدادات طريقة ضغط PPMd داخل أرشيف 7z. |
| [SevenZipPPMdCompressionSettings()](#SevenZipPPMdCompressionSettings--) | ينشئ إعدادات طريقة ضغط PPMd داخل أرشيف 7z مع ترتيب نموذج افتراضي وحجم المخصص الفرعي. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getMaxOrder()](#getMaxOrder--) | يحصل على الحد الأقصى للترتيب. |
| [getMethod()](#getMethod--) | يحصل على طريقة الضغط أو الفك. |
| [getSuballocatorSize()](#getSuballocatorSize--) | يحصل على حجم المخصص الفرعي بالميغابايت. |
### SevenZipPPMdCompressionSettings(int maxOrder, int suballocatorSize) {#SevenZipPPMdCompressionSettings-int-int-}
```
public SevenZipPPMdCompressionSettings(int maxOrder, int suballocatorSize)
```


ينشئ إعدادات طريقة ضغط PPMd داخل أرشيف 7z.

```

``````

try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings(4, 32)))) {
archive.createEntry(\"data.bin\", \"data.bin\");
archive.save("zipFile.zip");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| maxOrder | int | Maximum order.

Bigger model orders almost surely results in better compression and surely more memory and CPU usage. |
| suballocatorSize | int | Memory size in MB suballocator may consume.

The PPMd algorithm might need a lot of memory, especially when used on large files and/or used with large model order. If ppmd needs more memory than you give it, the compression will be worse. |

### SevenZipPPMdCompressionSettings() {#SevenZipPPMdCompressionSettings--}
```
public SevenZipPPMdCompressionSettings()
```


Instantiates settings for PPMd compression method within 7z archive with default model order and sub-allocator size.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings()))) {
         archive.createEntry("data.bin", "data.bin");
         archive.save("sevenZipFile.7z");
     }
 
```

ترتيب النموذج الافتراضي هو 6 وحجم المخصص الفرعي هو 16 ميغابايت.

### getMaxOrder() {#getMaxOrder--}
```
public final byte getMaxOrder()
```


يحصل على الحد الأقصى للترتيب.

**Returns:**
byte - الحد الأقصى للترتيب
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


يحصل على طريقة الضغط أو الفك.

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method
### getSuballocatorSize() {#getSuballocatorSize--}
```
public final int getSuballocatorSize()
```


يحصل على حجم المخصص الفرعي بالميغابايت.

**Returns:**
int - حجم المخصص الفرعي بالميغابايت
