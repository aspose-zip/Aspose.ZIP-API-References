---
title: AppleLz4CompressionSettings
second_title: Aspose.ZIP for Java API Reference
description: Settings for LZ4 compression within an Apple Archive .aar file.
type: docs
weight: 21
url: /java/com.aspose.zip/applelz4compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings)
```
public class AppleLz4CompressionSettings extends AppleCompressionSettings
```

Settings for LZ4 compression within an Apple Archive (.aar) file.
## Constructors

| Constructor | Description |
| --- | --- |
| [AppleLz4CompressionSettings(int blockSize)](#AppleLz4CompressionSettings-int-) | Initializes a new instance of the [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings) class. |
| [AppleLz4CompressionSettings()](#AppleLz4CompressionSettings--) | Initializes a new instance of the [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings) class with default parameters. |
## Methods

| Method | Description |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Gets the size of each compressed `pbz4`/`bv41` block. |
### AppleLz4CompressionSettings(int blockSize) {#AppleLz4CompressionSettings-int-}
```
public AppleLz4CompressionSettings(int blockSize)
```


Initializes a new instance of the [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| blockSize | int | The size of each compressed `pbz4`/`bv41` block. |

### AppleLz4CompressionSettings() {#AppleLz4CompressionSettings--}
```
public AppleLz4CompressionSettings()
```


Initializes a new instance of the [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings) class with default parameters.

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


Gets the size of each compressed `pbz4`/`bv41` block.

Value: The default value is 4 MiB.

**Returns:**
int - the size of each compressed `pbz4`/`bv41` block.
