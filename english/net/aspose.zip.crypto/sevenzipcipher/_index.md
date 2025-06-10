---
title: Class SevenZipCipher
second_title: Aspose.ZIP for .NET API Reference
description: Aspose.Zip.Crypto.SevenZipCipher class. Base class for AES cipher used for 7zip encryption
type: docs
weight: 240
url: /net/aspose.zip.crypto/sevenzipcipher/
---
## SevenZipCipher class

Base class for AES cipher used for 7-zip encryption.

```csharp
public abstract class SevenZipCipher : ICryptoTransform
```

## Properties

| Name | Description |
| --- | --- |
| abstract [CanReuseTransform](../../aspose.zip.crypto/sevenzipcipher/canreusetransform/) { get; } | Gets a value indicating whether the current transform can be reused. |
| abstract [CanTransformMultipleBlocks](../../aspose.zip.crypto/sevenzipcipher/cantransformmultipleblocks/) { get; } | Gets a value indicating whether multiple blocks can be transformed. |
| abstract [InputBlockSize](../../aspose.zip.crypto/sevenzipcipher/inputblocksize/) { get; } | Gets the input block size. |
| abstract [OutputBlockSize](../../aspose.zip.crypto/sevenzipcipher/outputblocksize/) { get; } | Gets the output block size. |

## Methods

| Name | Description |
| --- | --- |
| abstract [Dispose](../../aspose.zip.crypto/sevenzipcipher/dispose/)() | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| abstract [TransformBlock](../../aspose.zip.crypto/sevenzipcipher/transformblock/)(byte[], int, int, byte[], int) | Transforms the specified region of the input byte array and copies the resulting transform to the specified region of the output byte array. |
| abstract [TransformFinalBlock](../../aspose.zip.crypto/sevenzipcipher/transformfinalblock/)(byte[], int, int) | Transforms the specified region of the specified byte array. |

### See Also

* namespace [Aspose.Zip.Crypto](../../aspose.zip.crypto/)
* assembly [Aspose.Zip](../../)


