---
title: "AppleArchive.Save"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Méthode AppleArchive. Enregistre l'archive dans le flux fourni"
type: docs
weight: 90
url: /fr/net/aspose.zip.apple/applearchive/save/
---
## Save(Stream) {#save}

Enregistre l'archive dans le flux fourni.

```csharp
public void Save(Stream output)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sortie | Stream | Flux de destination. |

### Exceptions

| exception | condition |
| --- | --- |
| ObjectDisposedException | L'archive a été libérée. |
| ArgumentNullException | *output* est `null`. |
| ArgumentException | *output* n'est pas accessible en écriture. |
| ArgumentOutOfRangeException | La taille de bloc LZ4 ou Zlib configurée n'est pas positive. |
| NotSupportedException | Les paramètres de compression sont manquants ou non pris en charge, la composition directe utilise un flux non recherchable, ou la taille de l'entrée/archive dépasse les limites actuelles de l'Apple Archive. |

## Remarques

*output* must be writable. Some compression settings, such as LZ4, also require a seekable stream.

### Voir aussi

* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string) {#save_1}

Enregistre l'archive dans le fichier de destination fourni.

```csharp
public void Save(string destinationFileName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| destinationFileName | String | Le chemin de l'archive à créer. |

### Exceptions

| exception | condition |
| --- | --- |
| ObjectDisposedException | L'archive a été libérée. |
| ArgumentException | *destinationFileName* est invalide. |
| ArgumentNullException | *destinationFileName* est `null`. |
| ArgumentOutOfRangeException | La taille de bloc LZ4 ou Zlib configurée n'est pas positive. |
| NotSupportedException | Les paramètres de compression sont manquants ou non pris en charge, la composition directe utilise un flux non recherchable, ou la taille de l'entrée/archive dépasse les limites actuelles de l'Apple Archive. |

### Voir aussi

* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)


