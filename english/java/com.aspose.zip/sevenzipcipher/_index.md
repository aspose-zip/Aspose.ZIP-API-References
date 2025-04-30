---
title: SevenZipCipher
second_title: Aspose.ZIP for Java API Reference
description: Base class for AES cipher used for 7-zip encryption.
type: docs
weight: 76
url: /java/com.aspose.zip/sevenzipcipher/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.ms.System.Security.Cryptography.ICryptoTransform
```
public abstract class SevenZipCipher implements System.Security.Cryptography.ICryptoTransform
```

Base class for AES cipher used for 7-zip encryption.
## Methods

| Method | Description |
| --- | --- |
| [canReuseTransform()](#canReuseTransform--) | Gets a value indicating whether the current transform can be reused. |
| [canTransformMultipleBlocks()](#canTransformMultipleBlocks--) | Gets a value indicating whether multiple blocks can be transformed. |
| [dispose()](#dispose--) | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [getInputBlockSize()](#getInputBlockSize--) | Gets the input block size. |
| [getOutputBlockSize()](#getOutputBlockSize--) | Gets the output block size. |
| [transformBlock(byte[] inputBuffer, int inputOffset, int inputCount, byte[] outputBuffer, int outputOffset)](#transformBlock-byte---int-int-byte---int-) | Transforms the specified region of the input byte array and copies the resulting transform to the specified region of the output byte array. |
| [transformFinalBlock(byte[] inputBuffer, int inputOffset, int inputCount)](#transformFinalBlock-byte---int-int-) | Transforms the specified region of the specified byte array. |
### canReuseTransform() {#canReuseTransform--}
```
public abstract boolean canReuseTransform()
```


Gets a value indicating whether the current transform can be reused.

**Returns:**
boolean - a value indicating whether the current transform can be reused
### canTransformMultipleBlocks() {#canTransformMultipleBlocks--}
```
public abstract boolean canTransformMultipleBlocks()
```


Gets a value indicating whether multiple blocks can be transformed.

**Returns:**
boolean - a value indicating whether multiple blocks can be transformed
### dispose() {#dispose--}
```
public abstract void dispose()
```


Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources.

### getInputBlockSize() {#getInputBlockSize--}
```
public abstract int getInputBlockSize()
```


Gets the input block size.

**Returns:**
int - the input block size
### getOutputBlockSize() {#getOutputBlockSize--}
```
public abstract int getOutputBlockSize()
```


Gets the output block size.

**Returns:**
int - the output block size
### transformBlock(byte[] inputBuffer, int inputOffset, int inputCount, byte[] outputBuffer, int outputOffset) {#transformBlock-byte---int-int-byte---int-}
```
public abstract int transformBlock(byte[] inputBuffer, int inputOffset, int inputCount, byte[] outputBuffer, int outputOffset)
```


Transforms the specified region of the input byte array and copies the resulting transform to the specified region of the output byte array.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| inputBuffer | byte[] | the input for which to compute the transform |
| inputOffset | int | the offset into the input byte array from which to begin using data |
| inputCount | int | the number of bytes in the input byte array to use as data |
| outputBuffer | byte[] | the output to which to write the transform |
| outputOffset | int | the offset into the output byte array from which to begin writing data |

**Returns:**
int - the number of bytes written
### transformFinalBlock(byte[] inputBuffer, int inputOffset, int inputCount) {#transformFinalBlock-byte---int-int-}
```
public abstract byte[] transformFinalBlock(byte[] inputBuffer, int inputOffset, int inputCount)
```


Transforms the specified region of the specified byte array.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| inputBuffer | byte[] | the input for which to compute the transform |
| inputOffset | int | the offset into the input byte array from which to begin using data |
| inputCount | int | the number of bytes in the input byte array to use as data |

**Returns:**
byte[] - the computed transform
