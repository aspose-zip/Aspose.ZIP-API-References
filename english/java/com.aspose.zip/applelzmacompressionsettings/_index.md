---
title: AppleLzmaCompressionSettings
second_title: Aspose.ZIP for Java API Reference
description: Settings for LZMA compression within an Apple Archive .aar file.
type: docs
weight: 23
url: /java/com.aspose.zip/applelzmacompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings)
```
public class AppleLzmaCompressionSettings extends AppleCompressionSettings
```

Settings for LZMA compression within an Apple Archive (.aar) file.
## Constructors

| Constructor | Description |
| --- | --- |
| [AppleLzmaCompressionSettings(int blockSize)](#AppleLzmaCompressionSettings-int-) | Initializes a new instance of the [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) class. |
| [AppleLzmaCompressionSettings(int blockSize, int dictionarySize)](#AppleLzmaCompressionSettings-int-int-) | Initializes a new instance of the [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) class. |
| [AppleLzmaCompressionSettings(int blockSize, int dictionarySize, int fastBytes)](#AppleLzmaCompressionSettings-int-int-int-) | Initializes a new instance of the [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) class. |
| [AppleLzmaCompressionSettings()](#AppleLzmaCompressionSettings--) | Initializes a new instance of the [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) class with default parameters. |
## Methods

| Method | Description |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Gets the size of each data block before compression. |
| [getDictionarySize()](#getDictionarySize--) | Gets the dictionary size used for compression. |
| [getFastBytes()](#getFastBytes--) | Gets the number of fast bytes used for compression. |
### AppleLzmaCompressionSettings(int blockSize) {#AppleLzmaCompressionSettings-int-}
```
public AppleLzmaCompressionSettings(int blockSize)
```


Initializes a new instance of the [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| blockSize | int | The size of each data block before compression. |

### AppleLzmaCompressionSettings(int blockSize, int dictionarySize) {#AppleLzmaCompressionSettings-int-int-}
```
public AppleLzmaCompressionSettings(int blockSize, int dictionarySize)
```


Initializes a new instance of the [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| blockSize | int | The size of each data block before compression. |
| dictionarySize | int | The dictionary size used for compression. |

### AppleLzmaCompressionSettings(int blockSize, int dictionarySize, int fastBytes) {#AppleLzmaCompressionSettings-int-int-int-}
```
public AppleLzmaCompressionSettings(int blockSize, int dictionarySize, int fastBytes)
```


Initializes a new instance of the [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| blockSize | int | The size of each data block before compression. |
| dictionarySize | int | The dictionary size used for compression. |
| fastBytes | int | The number of fast bytes used for compression. |

### AppleLzmaCompressionSettings() {#AppleLzmaCompressionSettings--}
```
public AppleLzmaCompressionSettings()
```


Initializes a new instance of the [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) class with default parameters.

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


Gets the size of each data block before compression.

Value: The default value is 4 MiB.

**Returns:**
int - the size of each data block before compression.
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


Gets the dictionary size used for compression.

Value: The default value is 8 MiB.

**Returns:**
int - the dictionary size used for compression.
### getFastBytes() {#getFastBytes--}
```
public final int getFastBytes()
```


Gets the number of fast bytes used for compression.

Value: The default value is 32.

**Returns:**
int - the number of fast bytes used for compression.
