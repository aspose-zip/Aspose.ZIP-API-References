---
title: SevenZipCipher.TransformBlock
second_title: Aspose.ZIP for .NET API Reference
description: SevenZipCipher method. Transforms the specified region of the input byte array and copies the resulting transform to the specified region of the output byte array
type: docs
weight: 60
url: /net/aspose.zip.crypto/sevenzipcipher/transformblock/
---
## SevenZipCipher.TransformBlock method

Transforms the specified region of the input byte array and copies the resulting transform to the specified region of the output byte array.

```csharp
public abstract int TransformBlock(byte[] inputBuffer, int inputOffset, int inputCount, 
    byte[] outputBuffer, int outputOffset)
```

| Parameter | Type | Description |
| --- | --- | --- |
| inputBuffer | Byte[] | The input for which to compute the transform. |
| inputOffset | Int32 | The offset into the input byte array from which to begin using data. |
| inputCount | Int32 | The number of bytes in the input byte array to use as data. |
| outputBuffer | Byte[] | The output to which to write the transform. |
| outputOffset | Int32 | The offset into the output byte array from which to begin writing data. |

### See Also

* class [SevenZipCipher](../)
* namespace [Aspose.Zip.Crypto](../../sevenzipcipher/)
* assembly [Aspose.Zip](../../../)


