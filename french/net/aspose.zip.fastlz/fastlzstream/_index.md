---
title: "Classe FastLZStream"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Classe Aspose.Zip.FastLZ.FastLZStream. Un wrapper de flux qui compresse les données avec FastLZ. Implémente le motif décorateur."
type: docs
weight: 500
url: /fr/net/aspose.zip.fastlz/fastlzstream/
---
## FastLZStream class

Un wrapper de flux qui compresse les données avec FastLZ. Implémente le motif décorateur.

```csharp
public class FastLZStream : Stream
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [FastLZStream](fastlzstream/)(Stream, int) | Initialise une nouvelle instance de la classe `FastLZStream` préparée pour la compression. |

## Propriétés

| Nom | Description |
| --- | --- |
| override [CanRead](../../aspose.zip.fastlz/fastlzstream/canread/) { get; } | Obtient une valeur indiquant si le flux actuel prend en charge la lecture. |
| override [CanSeek](../../aspose.zip.fastlz/fastlzstream/canseek/) { get; } | Obtient une valeur indiquant si le flux actuel prend en charge le déplacement. |
| override [CanWrite](../../aspose.zip.fastlz/fastlzstream/canwrite/) { get; } | Obtient une valeur indiquant si le flux actuel prend en charge l'écriture. |
| override [Length](../../aspose.zip.fastlz/fastlzstream/length/) { get; } | Obtient la longueur en octets du flux. |
| override [Position](../../aspose.zip.fastlz/fastlzstream/position/) { get; set; } | Obtient ou définit la position dans le flux actuel. |

## Méthodes

| Nom | Description |
| --- | --- |
| override [Close](../../aspose.zip.fastlz/fastlzstream/close/)() | Ferme le flux actuel et libère toutes les ressources (telles que les sockets et les poignées de fichiers) associées au flux actuel. |
| override [Flush](../../aspose.zip.fastlz/fastlzstream/flush/)() | Vide tous les tampons de ce flux et force les données tamponnées à être écrites sur le dispositif sous-jacent. |
| override [Read](../../aspose.zip.fastlz/fastlzstream/read/)(byte[], int, int) | Lit une séquence d'octets depuis le flux et avance la position dans le flux du nombre d'octets lus. Non pris en charge. |
| override [Seek](../../aspose.zip.fastlz/fastlzstream/seek/)(long, SeekOrigin) | Définit la position dans le flux actuel. |
| override [SetLength](../../aspose.zip.fastlz/fastlzstream/setlength/)(long) | Définit la longueur du flux actuel. |
| override [Write](../../aspose.zip.fastlz/fastlzstream/write/)(byte[], int, int) | Écrit une séquence d'octets dans le flux de compression et avance la position actuelle dans ce flux du nombre d'octets écrits. |

### Voir aussi

* namespace [Aspose.Zip.FastLZ](../../aspose.zip.fastlz/)
* assembly [Aspose.Zip](../../)


