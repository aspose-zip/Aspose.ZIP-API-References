---
title: AppleLzfseCompressionSettings
second_title: Aspose.ZIP for Java API Reference
description: Settings for LZFSE compression within an Apple Archive .aar file.
type: docs
weight: 22
url: /java/com.aspose.zip/applelzfsecompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings)
```
public class AppleLzfseCompressionSettings extends AppleCompressionSettings
```

Settings for LZFSE compression within an Apple Archive (.aar) file.
## Constructors

| Constructor | Description |
| --- | --- |
| [AppleLzfseCompressionSettings(int blockSize)](#AppleLzfseCompressionSettings-int-) | Initializes a new instance of the [AppleLzfseCompressionSettings](../../com.aspose.zip/applelzfsecompressionsettings) class. |
| [AppleLzfseCompressionSettings()](#AppleLzfseCompressionSettings--) | Initializes a new instance of the [AppleLzfseCompressionSettings](../../com.aspose.zip/applelzfsecompressionsettings) class with default parameters. |
## Methods

| Method | Description |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Gets the size of each data block before compression. |
### AppleLzfseCompressionSettings(int blockSize) {#AppleLzfseCompressionSettings-int-}
```
public AppleLzfseCompressionSettings(int blockSize)
```


Initializes a new instance of the [AppleLzfseCompressionSettings](../../com.aspose.zip/applelzfsecompressionsettings) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| blockSize | int | The size of each data block before compression. |

### AppleLzfseCompressionSettings() {#AppleLzfseCompressionSettings--}
```
public AppleLzfseCompressionSettings()
```


Initializes a new instance of the [AppleLzfseCompressionSettings](../../com.aspose.zip/applelzfsecompressionsettings) class with default parameters.

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


Gets the size of each data block before compression.

Value: The default value is 4 MiB.

**Returns:**
int - the size of each data block before compression.
