---
title: "Classe ArjArchive"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Classe Aspose.Zip.Arj.ArjArchive. Cette classe représente un fichier d'archive ARJ"
type: docs
weight: 250
url: /fr/net/aspose.zip.arj/arjarchive/
---
## ArjArchive class

Cette classe représente un fichier d'archive ARJ.

```csharp
public class ArjArchive : IArchive
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [ArjArchive](arjarchive/#constructor)(Stream, ArjLoadOptions) | Initialise une nouvelle instance de la classe `ArjArchive` et compose une liste d'entrées pouvant être extraites de l'archive. |
| [ArjArchive](arjarchive/#constructor_1)(string, ArjLoadOptions) | Initialise une nouvelle instance de la classe `ArjArchive` et compose une liste d'entrées pouvant être extraites de l'archive. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Commentary](../../aspose.zip.arj/arjarchive/commentary/) { get; } | Obtient le commentaire. |
| [Entries](../../aspose.zip.arj/arjarchive/entries/) { get; } | Obtient les entrées de type [`ArjEntryPlain`](../arjentryplain/) constituant l'archive ARJ. |
| [Name](../../aspose.zip.arj/arjarchive/name/) { get; } | Obtient le nom d'origine. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Dispose](../../aspose.zip.arj/arjarchive/dispose/)() | Effectue les tâches définies par l'application associées à la libération, la remise ou la réinitialisation des ressources non gérées. |
| [ExtractToDirectory](../../aspose.zip.arj/arjarchive/extracttodirectory/)(string) | Extrait toutes les entrées vers le répertoire spécifié. |

## Remarques

Seules les méthodes de compression suivantes sont prises en charge :

**Method**

**Explanation**

**0**

Non compressé

**1**

Combinaison de LZ77 et de codage Huffman adaptatif. Meilleur taux de compression.

**2**

Combinaison de LZ77 et de codage Huffman adaptatif.

**3**

Combinaison de LZ77 et de codage Huffman adaptatif. Meilleure vitesse.

### Voir aussi

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Arj](../../aspose.zip.arj/)
* assembly [Aspose.Zip](../../)


