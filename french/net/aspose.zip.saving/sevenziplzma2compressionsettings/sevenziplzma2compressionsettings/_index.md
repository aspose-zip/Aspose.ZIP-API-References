---
title: SevenZipLZMA2CompressionSettings.SevenZipLZMA2CompressionSettings
second_title: Référence de l'API Aspose.ZIP pour .NET
description: SevenZipLZMA2CompressionSettings constructeur. Instancie les paramètres de la méthode de compression LZMA2 dans larchive 7z.
type: docs
weight: 10
url: /fr/net/aspose.zip.saving/sevenziplzma2compressionsettings/sevenziplzma2compressionsettings/
---
## SevenZipLZMA2CompressionSettings(int) {#constructor}

Instancie les paramètres de la méthode de compression LZMA2 dans l'archive 7z.

```csharp
public SevenZipLZMA2CompressionSettings(int dictionarySize = 16777216)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| dictionarySize | Int32 | Taille du tampon d'historique, doit être comprise entre 4096 et 1073741824. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentOutOfRangeException | *dictionarySize* est trop grand ou trop petit. |

### Remarques

Plus le dictionnaire est volumineux, meilleur est généralement le taux de compression, mais les dictionnaires plus volumineux que les données non compressées sont un gaspillage de RAM.

### Voir également

* class [SevenZipLZMA2CompressionSettings](../)
* espace de noms [Aspose.Zip.Saving](../../sevenziplzma2compressionsettings/)
* Assemblée [Aspose.Zip](../../../)

---

## SevenZipLZMA2CompressionSettings(int, int) {#constructor_1}

Instancie les paramètres de la méthode de compression LZMA2 dans l'archive 7z.

```csharp
public SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes = 32)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| dictionarySize | Int32 | Taille du tampon d'historique, doit être comprise entre 4096 et 1073741824. |
| fastBytes | Int32 | Contrôle le nombre d'octets rapides utilisés par les compresseurs LZMA2. Un plus grand nombre d'octets rapides peut fournir un meilleur taux de compression au détriment de la vitesse de compression. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentOutOfRangeException | *dictionarySize* est trop grand ou trop petit, ou*fastBytes* est trop grand ou trop petit. |

### Remarques

Plus le dictionnaire est volumineux, meilleur est généralement le taux de compression, mais les dictionnaires plus volumineux que les données non compressées sont un gaspillage de RAM.

### Voir également

* class [SevenZipLZMA2CompressionSettings](../)
* espace de noms [Aspose.Zip.Saving](../../sevenziplzma2compressionsettings/)
* Assemblée [Aspose.Zip](../../../)


