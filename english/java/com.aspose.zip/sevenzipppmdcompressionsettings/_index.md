---
title: SevenZipPPMdCompressionSettings
second_title: Aspose.ZIP for Java API Reference
description: Settings for PPMd compression method within 7z archive.
type: docs
weight: 82
url: /java/com.aspose.zip/sevenzipppmdcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public final class SevenZipPPMdCompressionSettings extends SevenZipCompressionSettings
```

Settings for PPMd compression method within 7z archive.
## Constructors

| Constructor | Description |
| --- | --- |
| [SevenZipPPMdCompressionSettings(int maxOrder, int suballocatorSize)](#SevenZipPPMdCompressionSettings-int-int-) | Instantiates settings for PPMd compression method within 7z archive. |
| [SevenZipPPMdCompressionSettings()](#SevenZipPPMdCompressionSettings--) | Instantiates settings for PPMd compression method within 7z archive with default model order and sub-allocator size. |
## Methods

| Method | Description |
| --- | --- |
| [getMaxOrder()](#getMaxOrder--) | Gets the maximum order. |
| [getMethod()](#getMethod--) | Gets compression or decompression method. |
| [getSuballocatorSize()](#getSuballocatorSize--) | Gets the sub-allocator size in MB. |
### SevenZipPPMdCompressionSettings(int maxOrder, int suballocatorSize) {#SevenZipPPMdCompressionSettings-int-int-}
```
public SevenZipPPMdCompressionSettings(int maxOrder, int suballocatorSize)
```


Instantiates settings for PPMd compression method within 7z archive.

```

     try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings(4, 32)))) {
         archive.createEntry("data.bin", "data.bin");
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

     try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings()))) {
         archive.createEntry("data.bin", "data.bin");
         archive.save("sevenZipFile.7z");
     }
 
```

The default model order is 6 and sub-allocator size is 16MB.

### getMaxOrder() {#getMaxOrder--}
```
public final byte getMaxOrder()
```


Gets the maximum order.

**Returns:**
byte - the maximum order
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


Gets compression or decompression method.

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method
### getSuballocatorSize() {#getSuballocatorSize--}
```
public final int getSuballocatorSize()
```


Gets the sub-allocator size in MB.

**Returns:**
int - the sub-allocator size in MB
