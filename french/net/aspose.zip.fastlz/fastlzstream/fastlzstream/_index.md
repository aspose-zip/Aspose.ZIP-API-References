---
title: "FastLZStream.FastLZStream"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Constructeur FastLZStream. Initialise une nouvelle instance de la classe FastLZStream préparée pour la compression"
type: docs
weight: 10
url: /fr/net/aspose.zip.fastlz/fastlzstream/fastlzstream/
---
## FastLZStream constructor

Initialise une nouvelle instance de la classe [`FastLZStream`](../) préparée pour la compression.

```csharp
public FastLZStream(Stream stream, int compressionLevel)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| stream | Stream | Le flux utilisé pour enregistrer les données compressées. |
| compressionLevel | Int32 | Utilisez 1 pour une compression plus rapide, utilisez 2 pour un meilleur taux de compression. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *stream* est nul. |
| ArgumentException | *stream* ne prend pas en charge l'écriture. |
| ArgumentOutOfRangeException | *compressionLevel* est supérieur à 2 ou inférieur à 1. |

### Voir aussi

* class [FastLZStream](../)
* namespace [Aspose.Zip.FastLZ](../../fastlzstream/)
* assembly [Aspose.Zip](../../../)


