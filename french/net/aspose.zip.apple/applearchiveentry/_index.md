---
title: "Classe AppleArchiveEntry"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Classe Aspose.Zip.Apple.AppleArchiveEntry. Représente une entrée du système de fichiers dans un AppleArchive"
type: docs
weight: 70
url: /fr/net/aspose.zip.apple/applearchiveentry/
---
## AppleArchiveEntry class

Représente une entrée du système de fichiers dans un [`AppleArchive`](../applearchive/).

```csharp
public sealed class AppleArchiveEntry : IArchiveFileEntry
```

## Propriétés

| Nom | Description |
| --- | --- |
| [IsDirectory](../../aspose.zip.apple/applearchiveentry/isdirectory/) { get; } | Obtient une valeur indiquant si l'entrée représente un répertoire. |
| [IsSymbolicLink](../../aspose.zip.apple/applearchiveentry/issymboliclink/) { get; } | Obtient une valeur indiquant si l'entrée représente un lien symbolique. |
| [Length](../../aspose.zip.apple/applearchiveentry/length/) { get; } | Obtient la longueur non compressée de l'entrée en octets. |
| [Name](../../aspose.zip.apple/applearchiveentry/name/) { get; } | Obtient le chemin de l'entrée à l'intérieur de l'archive. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Extract](../../aspose.zip.apple/applearchiveentry/extract/#extract_1)(Stream) | Extrait l'entrée vers le flux fourni. |
| [Extract](../../aspose.zip.apple/applearchiveentry/extract/#extract)(string) | Extrait l'entrée dans le système de fichiers au chemin fourni. |
| [Open](../../aspose.zip.apple/applearchiveentry/open/)() | Ouvre l'entrée pour l'extraction et fournit un flux contenant le contenu de l'entrée. |

## Remarques

Une instance de cette classe peut représenter un fichier ordinaire, un répertoire ou un lien symbolique analysé à partir d'une Apple Archive existante, ou un fichier ou répertoire ajouté à une archive en cours de composition.

### Voir aussi

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Apple](../../aspose.zip.apple/)
* assembly [Aspose.Zip](../../)


