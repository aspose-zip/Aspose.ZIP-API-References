---
title: Class SevenZipCipher
second_title: Référence de l'API Aspose.ZIP pour .NET
description: Aspose.Zip.Crypto.SevenZipCipher classe. Classe de base pour le chiffrement AES utilisé pour le chiffrement 7zip.
type: docs
weight: 190
url: /fr/net/aspose.zip.crypto/sevenzipcipher/
---
## SevenZipCipher class

Classe de base pour le chiffrement AES utilisé pour le chiffrement 7-zip.

```csharp
public abstract class SevenZipCipher : ICryptoTransform
```

## Propriétés

| Nom | La description |
| --- | --- |
| abstract [CanReuseTransform](../../aspose.zip.crypto/sevenzipcipher/canreusetransform/) { get; } | Obtient une valeur indiquant si la transformation actuelle peut être réutilisée. |
| abstract [CanTransformMultipleBlocks](../../aspose.zip.crypto/sevenzipcipher/cantransformmultipleblocks/) { get; } | Obtient une valeur indiquant si plusieurs blocs peuvent être transformés. |
| abstract [InputBlockSize](../../aspose.zip.crypto/sevenzipcipher/inputblocksize/) { get; } | Obtient la taille du bloc d'entrée. |
| abstract [OutputBlockSize](../../aspose.zip.crypto/sevenzipcipher/outputblocksize/) { get; } | Obtient la taille du bloc de sortie. |

## Méthodes

| Nom | La description |
| --- | --- |
| abstract [Dispose](../../aspose.zip.crypto/sevenzipcipher/dispose/)() | Effectue des tâches définies par l'application associées à la libération, à la libération ou à la réinitialisation des ressources non gérées. |
| abstract [TransformBlock](../../aspose.zip.crypto/sevenzipcipher/transformblock/)(byte[], int, int, byte[], int) | Transforme la région spécifiée du tableau d'octets d'entrée et copie la transformation résultante dans la région spécifiée du tableau d'octets de sortie. |
| abstract [TransformFinalBlock](../../aspose.zip.crypto/sevenzipcipher/transformfinalblock/)(byte[], int, int) | Transforme la région spécifiée du tableau d'octets spécifié. |

### Voir également

* espace de noms [Aspose.Zip.Crypto](../../aspose.zip.crypto/)
* Assemblée [Aspose.Zip](../../)


