---
title: Class SevenZipCipher
second_title: Aspose.ZIP für .NET-API-Referenz
description: Aspose.Zip.Crypto.SevenZipCipher klas. Basisklasse für AESChiffre die für 7ZipVerschlüsselung verwendet wird.
type: docs
weight: 190
url: /de/net/aspose.zip.crypto/sevenzipcipher/
---
## SevenZipCipher class

Basisklasse für AES-Chiffre, die für 7-Zip-Verschlüsselung verwendet wird.

```csharp
public abstract class SevenZipCipher : ICryptoTransform
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| abstract [CanReuseTransform](../../aspose.zip.crypto/sevenzipcipher/canreusetransform/) { get; } | Ruft einen Wert ab, der angibt, ob die aktuelle Transformation wiederverwendet werden kann. |
| abstract [CanTransformMultipleBlocks](../../aspose.zip.crypto/sevenzipcipher/cantransformmultipleblocks/) { get; } | Ruft einen Wert ab, der angibt, ob mehrere Blöcke transformiert werden können. |
| abstract [InputBlockSize](../../aspose.zip.crypto/sevenzipcipher/inputblocksize/) { get; } | Ruft die Eingangsblockgröße ab. |
| abstract [OutputBlockSize](../../aspose.zip.crypto/sevenzipcipher/outputblocksize/) { get; } | Ruft die Ausgangsblockgröße ab. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| abstract [Dispose](../../aspose.zip.crypto/sevenzipcipher/dispose/)() | Führt anwendungsdefinierte Aufgaben aus, die mit dem Freigeben, Freigeben oder Zurücksetzen nicht verwalteter Ressourcen verbunden sind. |
| abstract [TransformBlock](../../aspose.zip.crypto/sevenzipcipher/transformblock/)(byte[], int, int, byte[], int) | Transformiert den angegebenen Bereich des Eingabe-Byte-Arrays und kopiert die resultierende Transformation in den angegebenen Bereich des Ausgabe-Byte-Arrays. |
| abstract [TransformFinalBlock](../../aspose.zip.crypto/sevenzipcipher/transformfinalblock/)(byte[], int, int) | Transformiert den angegebenen Bereich des angegebenen Byte-Arrays. |

### Siehe auch

* namensraum [Aspose.Zip.Crypto](../../aspose.zip.crypto/)
* Montage [Aspose.Zip](../../)


