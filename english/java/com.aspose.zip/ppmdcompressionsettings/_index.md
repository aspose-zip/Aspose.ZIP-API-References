---
title: PPMdCompressionSettings
second_title: Aspose.ZIP for Java API Reference
description: Settings for PPMd compression method.
type: docs
weight: 61
url: /java/com.aspose.zip/ppmdcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class PPMdCompressionSettings extends CompressionSettings
```

Settings for PPMd compression method.

PPMd is a data compression algorithm developed by Dmitry Shkarin. This algorithm is based on predictive phrase matching on multiple order contexts.
## Constructors

| Constructor | Description |
| --- | --- |
| [PPMdCompressionSettings(int modelOrder, int suballocatorSize)](#PPMdCompressionSettings-int-int-) | Initializes a new instance of the [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings) class. |
| [PPMdCompressionSettings()](#PPMdCompressionSettings--) | Initializes a new instance of the [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings) class with default model order and sub-allocator size. |
## Methods

| Method | Description |
| --- | --- |
| [getModelOrder()](#getModelOrder--) | Gets the order of the model. |
| [getSuballocatorSize()](#getSuballocatorSize--) | Gets the sub-allocator size in MB. |
### PPMdCompressionSettings(int modelOrder, int suballocatorSize) {#PPMdCompressionSettings-int-int-}
```
public PPMdCompressionSettings(int modelOrder, int suballocatorSize)
```


Initializes a new instance of the [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings) class.

```

     try (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings(4, 10)))) {
         archive.createEntry("data.bin", "data.bin");
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

     try (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings()))) {
         archive.createEntry("data.bin", "data.bin");
         archive.save("zipFile.zip");
     }
 
```

The default model order is 8, and the sub-allocator size is 50MB.

### getModelOrder() {#getModelOrder--}
```
public final int getModelOrder()
```


Gets the order of the model.

**Returns:**
int - the order of the model
### getSuballocatorSize() {#getSuballocatorSize--}
```
public final int getSuballocatorSize()
```


Gets the sub-allocator size in MB.

**Returns:**
int - the sub-allocator size in MB
