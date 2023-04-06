---
title: Class SevenZipCipher
second_title: Aspose.ZIP för .NET API-referens
description: Aspose.Zip.Crypto.SevenZipCipher klass. Basklass för AESchiffer som används för 7zipkryptering.
type: docs
weight: 190
url: /sv/net/aspose.zip.crypto/sevenzipcipher/
---
## SevenZipCipher class

Basklass för AES-chiffer som används för 7-zip-kryptering.

```csharp
public abstract class SevenZipCipher : ICryptoTransform
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| abstract [CanReuseTransform](../../aspose.zip.crypto/sevenzipcipher/canreusetransform/) { get; } | Får ett värde som indikerar om den aktuella transformationen kan återanvändas. |
| abstract [CanTransformMultipleBlocks](../../aspose.zip.crypto/sevenzipcipher/cantransformmultipleblocks/) { get; } | Får ett värde som indikerar om flera block kan transformeras. |
| abstract [InputBlockSize](../../aspose.zip.crypto/sevenzipcipher/inputblocksize/) { get; } | Hämtar indatablockstorleken. |
| abstract [OutputBlockSize](../../aspose.zip.crypto/sevenzipcipher/outputblocksize/) { get; } | Hämtar utdatablockstorleken. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| abstract [Dispose](../../aspose.zip.crypto/sevenzipcipher/dispose/)() | Utför programdefinierade uppgifter associerade med att frigöra, frigöra eller återställa ohanterade resurser. |
| abstract [TransformBlock](../../aspose.zip.crypto/sevenzipcipher/transformblock/)(byte[], int, int, byte[], int) | Transformerar den angivna regionen i den inmatade bytematrisen och kopierar den resulterande transformationen till den specificerade regionen i den utgående bytematrisen. |
| abstract [TransformFinalBlock](../../aspose.zip.crypto/sevenzipcipher/transformfinalblock/)(byte[], int, int) | Transformerar den angivna regionen i den angivna byte-arrayen. |

### Se även

* namnutrymme [Aspose.Zip.Crypto](../../aspose.zip.crypto/)
* hopsättning [Aspose.Zip](../../)


