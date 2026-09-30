---
title: "FastLZStream.Read"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "FastLZStream method. Lit une séquence d'octets du flux et avance la position dans le flux du nombre d'octets lus. Non pris en charge"
type: docs
weight: 90
url: /fr/net/aspose.zip.fastlz/fastlzstream/read/
---
## FastLZStream.Read method

Lit une séquence d'octets depuis le flux et avance la position dans le flux du nombre d'octets lus. Non pris en charge.

```csharp
public override int Read(byte[] buffer, int offset, int count)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| tampon | Byte[] | Un tableau d'octets. Lorsque cette méthode retourne, le tampon contient le tableau d'octets spécifié avec les valeurs entre offset et (offset + count - 1) remplacées par les octets lus depuis la source actuelle. |
| décalage | Int32 | Le décalage d'octet basé sur zéro dans le tampon à partir duquel commencer à stocker les données lues depuis le flux actuel. |
| count | Int32 | Le nombre maximal d'octets à lire depuis le flux actuel. |

### Valeur de retour

Le nombre total d'octets lus dans le tampon. Cela peut être inférieur au nombre d'octets demandé si autant d'octets ne sont pas disponibles actuellement, ou zéro (0) si la fin du flux a été atteinte.

### Exceptions

| exception | condition |
| --- | --- |
| NotSupportedException | L'opération n'est pas prise en charge. |

### Voir aussi

* class [FastLZStream](../)
* namespace [Aspose.Zip.FastLZ](../../fastlzstream/)
* assembly [Aspose.Zip](../../../)


