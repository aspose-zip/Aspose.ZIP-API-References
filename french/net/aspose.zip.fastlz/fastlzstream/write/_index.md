---
title: "FastLZStream.Write"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "FastLZStream method. Écrit une séquence d'octets dans le flux de compression et avance la position actuelle dans ce flux du nombre d'octets écrits"
type: docs
weight: 120
url: /fr/net/aspose.zip.fastlz/fastlzstream/write/
---
## FastLZStream.Write method

Écrit une séquence d'octets dans le flux de compression et avance la position actuelle dans ce flux du nombre d'octets écrits.

```csharp
public override void Write(byte[] buffer, int offset, int count)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| tampon | Byte[] | Un tableau d'octets. Cette méthode copie count octets du tampon vers le flux actuel. |
| décalage | Int32 | Le décalage d'octet basé sur zéro dans le tampon à partir duquel commencer à copier les octets vers le flux actuel. |
| count | Int32 | Le nombre d'octets à écrire dans le flux actuel. |

### Exceptions

| exception | condition |
| --- | --- |
| ObjectDisposedException | Lancée si le flux a été libéré. |
| ArgumentNullException | *buffer* est `null`. |

### Voir aussi

* class [FastLZStream](../)
* namespace [Aspose.Zip.FastLZ](../../fastlzstream/)
* assembly [Aspose.Zip](../../../)


