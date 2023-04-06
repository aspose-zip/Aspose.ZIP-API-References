---
title: Class SevenZipCipher
second_title: Riferimento API Aspose.ZIP per .NET
description: Aspose.Zip.Crypto.SevenZipCipher classe. Classe base per la crittografia AES utilizzata per la crittografia a 7 zip.
type: docs
weight: 190
url: /it/net/aspose.zip.crypto/sevenzipcipher/
---
## SevenZipCipher class

Classe base per la crittografia AES utilizzata per la crittografia a 7 zip.

```csharp
public abstract class SevenZipCipher : ICryptoTransform
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| abstract [CanReuseTransform](../../aspose.zip.crypto/sevenzipcipher/canreusetransform/) { get; } | Ottiene un valore che indica se la trasformazione corrente può essere riutilizzata. |
| abstract [CanTransformMultipleBlocks](../../aspose.zip.crypto/sevenzipcipher/cantransformmultipleblocks/) { get; } | Ottiene un valore che indica se più blocchi possono essere trasformati. |
| abstract [InputBlockSize](../../aspose.zip.crypto/sevenzipcipher/inputblocksize/) { get; } | Ottiene la dimensione del blocco di input. |
| abstract [OutputBlockSize](../../aspose.zip.crypto/sevenzipcipher/outputblocksize/) { get; } | Ottiene la dimensione del blocco di output. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| abstract [Dispose](../../aspose.zip.crypto/sevenzipcipher/dispose/)() | Esegue attività definite dall'applicazione associate alla liberazione, al rilascio o al ripristino di risorse non gestite. |
| abstract [TransformBlock](../../aspose.zip.crypto/sevenzipcipher/transformblock/)(byte[], int, int, byte[], int) | Trasforma l'area specificata della matrice di byte di input e copia la trasformazione risultante nell'area specificata della matrice di byte di output. |
| abstract [TransformFinalBlock](../../aspose.zip.crypto/sevenzipcipher/transformfinalblock/)(byte[], int, int) | Trasforma la regione specificata dell'array di byte specificato. |

### Guarda anche

* spazio dei nomi [Aspose.Zip.Crypto](../../aspose.zip.crypto/)
* assemblea [Aspose.Zip](../../)


