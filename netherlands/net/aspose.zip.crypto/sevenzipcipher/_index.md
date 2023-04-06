---
title: Class SevenZipCipher
second_title: Aspose.ZIP voor .NET API-referentie
description: Aspose.Zip.Crypto.SevenZipCipher klas. Basisklasse voor AEScodering gebruikt voor 7zipencryptie.
type: docs
weight: 190
url: /nl/net/aspose.zip.crypto/sevenzipcipher/
---
## SevenZipCipher class

Basisklasse voor AES-codering gebruikt voor 7-zip-encryptie.

```csharp
public abstract class SevenZipCipher : ICryptoTransform
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| abstract [CanReuseTransform](../../aspose.zip.crypto/sevenzipcipher/canreusetransform/) { get; } | Krijgt een waarde die aangeeft of de huidige transformatie opnieuw kan worden gebruikt. |
| abstract [CanTransformMultipleBlocks](../../aspose.zip.crypto/sevenzipcipher/cantransformmultipleblocks/) { get; } | Krijgt een waarde die aangeeft of meerdere blokken kunnen worden getransformeerd. |
| abstract [InputBlockSize](../../aspose.zip.crypto/sevenzipcipher/inputblocksize/) { get; } | Haalt de invoerblokgrootte op. |
| abstract [OutputBlockSize](../../aspose.zip.crypto/sevenzipcipher/outputblocksize/) { get; } | Haalt de grootte van het uitvoerblok op. |

## methoden

| Naam | Beschrijving |
| --- | --- |
| abstract [Dispose](../../aspose.zip.crypto/sevenzipcipher/dispose/)() | Voert door de toepassing gedefinieerde taken uit die verband houden met het vrijmaken, vrijgeven of resetten van onbeheerde bronnen. |
| abstract [TransformBlock](../../aspose.zip.crypto/sevenzipcipher/transformblock/)(byte[], int, int, byte[], int) | Transformeert het gespecificeerde gebied van de invoerbytearray en kopieert de resulterende transformatie naar het gespecificeerde gebied van de uitvoerbytearray. |
| abstract [TransformFinalBlock](../../aspose.zip.crypto/sevenzipcipher/transformfinalblock/)(byte[], int, int) | Transformeert het opgegeven gebied van de opgegeven byte-array. |

### Zie ook

* naamruimte [Aspose.Zip.Crypto](../../aspose.zip.crypto/)
* montage [Aspose.Zip](../../)


