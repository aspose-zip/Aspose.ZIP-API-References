---
title: "Classe LhaArchive"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Aspose.Zip.Lha.LhaArchive classe. Cette classe représente un fichier d'archive LHA .lzh"
type: docs
weight: 630
url: /fr/net/aspose.zip.lha/lhaarchive/
---
## LhaArchive class

Cette classe représente un fichier d'archive LHA (.lzh).

```csharp
public class LhaArchive : IArchive
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [LhaArchive](lhaarchive/#constructor)(Stream, LhaLoadOptions) | Initialise une nouvelle instance de la classe `LhaArchive` et compose une liste d'entrées pouvant être extraites de l'archive. |
| [LhaArchive](lhaarchive/#constructor_1)(string, LhaLoadOptions) | Initialise une nouvelle instance de la classe `LhaArchive` et compose une liste d'entrées pouvant être extraites de l'archive. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Entries](../../aspose.zip.lha/lhaarchive/entries/) { get; } | Obtient les entrées de fichiers du type [`LhaArchiveEntry`](../lhaarchiveentry/) constituant l'archive. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Dispose](../../aspose.zip.lha/lhaarchive/dispose/)() |  |
| [ExtractToDirectory](../../aspose.zip.lha/lhaarchive/extracttodirectory/)(string) | Extrait tous les fichiers et répertoires de l'archive vers le répertoire fourni. |

## Remarques

Seules les méthodes de compression suivantes sont prises en charge :

**Method**

**Explanation**

**lh0**

Non compressé

**lh4**

Dictionnaire glissant de 8 KiB et Huffman statique

**lh5**

Dictionnaire glissant de 16 KiB et Huffman statique

**lh6**

Dictionnaire glissant de 64 KiB et Huffman statique

**lh7**

Dictionnaire glissant de 128 KiB et Huffman statique

**lhx**

Dictionnaire glissant de 1 Mib et Huffman statique

**lhd**

Répertoire

### Voir aussi

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Lha](../../aspose.zip.lha/)
* assembly [Aspose.Zip](../../)


