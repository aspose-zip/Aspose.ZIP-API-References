---
title: ParallelOptions
second_title: Aspose.ZIP for Java API Reference
description: Options for parallel compression.
type: docs
weight: 69
url: /java/com.aspose.zip/paralleloptions/
---

**Inheritance:**
java.lang.Object
```
public class ParallelOptions
```

Options for parallel compression.

```

    try (Archive archive = new Archive()) {
        archive.createEntries("DirToCompress");
        ParallelOptions parallelOptions = new ParallelOptions();
        parallelOptions.setParallelCompressInMemory(mode);
        parallelOptions.setAvailableMemorySize(4000);
        ArchiveSaveOptions archiveSaveOptions = new ArchiveSaveOptions();
        archiveSaveOptions.setParallelOptions(parallelOptions);
        archive.save("archive.zip", archiveSaveOptions);
    }
 
```

These options manage simultaneous compression by several CPU cores.
## Constructors

| Constructor | Description |
| --- | --- |
| [ParallelOptions()](#ParallelOptions--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getAvailableMemorySize()](#getAvailableMemorySize--) | Gets memory estimate in megabytes available to accomodate compressed entries without a swap to disk. |
| [getParallelCompressInMemory()](#getParallelCompressInMemory--) | Gets value indicating how parallel approach to be used. |
| [setAvailableMemorySize(int value)](#setAvailableMemorySize-int-) | Sets memory estimate in megabytes available to accomodate compressed entries without a swap to disk. |
| [setParallelCompressInMemory(ParallelCompressionMode value)](#setParallelCompressInMemory-com.aspose.zip.ParallelCompressionMode-) | Sets value indicating how parallel approach to be used. |
### ParallelOptions() {#ParallelOptions--}
```
public ParallelOptions()
```


### getAvailableMemorySize() {#getAvailableMemorySize--}
```
public final int getAvailableMemorySize()
```


Gets memory estimate in megabytes available to accomodate compressed entries without a swap to disk. This value only makes sense if [getParallelCompressInMemory()](../../com.aspose.zip/paralleloptions\#getParallelCompressInMemory--) setting is in [ParallelCompressionMode.Auto](../../com.aspose.zip/parallelcompressionmode\#Auto) mode.

This value is used to calculate the biggest size of entry that can be compressed in parallel with others. All entries above the calculated threshold will be compressed sequentially. It is safe to have [getAvailableMemorySize()](../../com.aspose.zip/paralleloptions\#getAvailableMemorySize--) property as big as free RAM and even bigger. By default it is assumed you have at least 200MB per CPU core.

**Returns:**
int - memory estimate in megabytes available to accomodate compressed entries without a swap to disk.
### getParallelCompressInMemory() {#getParallelCompressInMemory--}
```
public final ParallelCompressionMode getParallelCompressInMemory()
```


Gets value indicating how parallel approach to be used.

**Returns:**
[ParallelCompressionMode](../../com.aspose.zip/parallelcompressionmode) - value indicating how parallel approach to be used.
### setAvailableMemorySize(int value) {#setAvailableMemorySize-int-}
```
public final void setAvailableMemorySize(int value)
```


Sets memory estimate in megabytes available to accomodate compressed entries without a swap to disk. This value only makes sense if [getParallelCompressInMemory()](../../com.aspose.zip/paralleloptions\#getParallelCompressInMemory--) setting is in [ParallelCompressionMode.Auto](../../com.aspose.zip/parallelcompressionmode\#Auto) mode.

This value is used to calculate the biggest size of entry that can be compressed in parallel with others. All entries above the calculated threshold will be compressed sequentially. It is safe to have [getAvailableMemorySize()](../../com.aspose.zip/paralleloptions\#getAvailableMemorySize--) property as big as free RAM and even bigger. By default it is assumed you have at least 200MB per CPU core.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | memory estimate in megabytes available to accomodate compressed entries without a swap to disk. |

### setParallelCompressInMemory(ParallelCompressionMode value) {#setParallelCompressInMemory-com.aspose.zip.ParallelCompressionMode-}
```
public final void setParallelCompressInMemory(ParallelCompressionMode value)
```


Sets value indicating how parallel approach to be used.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ParallelCompressionMode](../../com.aspose.zip/parallelcompressionmode) | value indicating how parallel approach to be used. |

