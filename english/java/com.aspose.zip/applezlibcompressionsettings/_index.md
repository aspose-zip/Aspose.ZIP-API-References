---
title: AppleZlibCompressionSettings
second_title: Aspose.ZIP for Java API Reference
description: Settings for Zlib compression within an Apple Archive .aar file.
type: docs
weight: 25
url: /java/com.aspose.zip/applezlibcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings)
```
public class AppleZlibCompressionSettings extends AppleCompressionSettings
```

Settings for Zlib compression within an Apple Archive (.aar) file.
## Constructors

| Constructor | Description |
| --- | --- |
| [AppleZlibCompressionSettings(int blockSize)](#AppleZlibCompressionSettings-int-) | Initializes a new instance of the [AppleZlibCompressionSettings](../../com.aspose.zip/applezlibcompressionsettings) class. |
| [AppleZlibCompressionSettings()](#AppleZlibCompressionSettings--) | Initializes a new instance of the [AppleZlibCompressionSettings](../../com.aspose.zip/applezlibcompressionsettings) class with default parameters. |
## Methods

| Method | Description |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Gets the size of each data block before compression. |
### AppleZlibCompressionSettings(int blockSize) {#AppleZlibCompressionSettings-int-}
```
public AppleZlibCompressionSettings(int blockSize)
```


Initializes a new instance of the [AppleZlibCompressionSettings](../../com.aspose.zip/applezlibcompressionsettings) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| blockSize | int | The size of each data block before compression. |

### AppleZlibCompressionSettings() {#AppleZlibCompressionSettings--}
```
public AppleZlibCompressionSettings()
```


Initializes a new instance of the [AppleZlibCompressionSettings](../../com.aspose.zip/applezlibcompressionsettings) class with default parameters.

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


Gets the size of each data block before compression.

Value: The default value is 4 MiB.

**Returns:**
int - the size of each data block before compression.
