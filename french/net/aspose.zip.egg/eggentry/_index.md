---
title: "Classe EggEntry"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Aspose.Zip.Egg.EggEntry classe. Représente une entrée de fichier dans une archive EGG avec toutes ses métadonnées"
type: docs
weight: 470
url: /fr/net/aspose.zip.egg/eggentry/
---
## EggEntry class

Représente une entrée de fichier dans une archive EGG avec toutes ses métadonnées.

```csharp
public abstract class EggEntry : IArchiveFileEntry
```

## Propriétés

| Nom | Description |
| --- | --- |
| [CompressedSize](../../aspose.zip.egg/eggentry/compressedsize/) { get; } | Obtient la taille compressée de l'entrée. |
| [IsDirectory](../../aspose.zip.egg/eggentry/isdirectory/) { get; } | Obtient une valeur indiquant si cette entrée représente un répertoire. |
| [Length](../../aspose.zip.egg/eggentry/length/) { get; } |  |
| [ModificationTime](../../aspose.zip.egg/eggentry/modificationtime/) { get; } | Obtient ou définit la date et l'heure de dernière modification. |
| [Name](../../aspose.zip.egg/eggentry/name/) { get; } | Obtient le nom de l'entrée dans l'archive. |
| [UncompressedSize](../../aspose.zip.egg/eggentry/uncompressedsize/) { get; } | Obtient la taille non compressée de l'entrée. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Extract](../../aspose.zip.egg/eggentry/extract/#extract_1)(Stream) | Extrait l'entrée vers le flux fourni. |
| [Extract](../../aspose.zip.egg/eggentry/extract/#extract)(string) | Extrait l'entrée dans le système de fichiers au chemin fourni. |
| [Open](../../aspose.zip.egg/eggentry/open/)() | Ouvre l'entrée pour l'extraction et fournit un flux avec le contenu décompressé de l'entrée. |

### Voir aussi

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Egg](../../aspose.zip.egg/)
* assembly [Aspose.Zip](../../)


