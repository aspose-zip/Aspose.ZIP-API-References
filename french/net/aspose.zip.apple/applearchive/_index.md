---
title: "Classe AppleArchive"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Classe Aspose.Zip.Apple.AppleArchive. Cette classe représente un fichier Apple Archive .aar. Utilisez‑la pour composer des fichiers Apple Archive."
type: docs
weight: 60
url: /fr/net/aspose.zip.apple/applearchive/
---
## AppleArchive class

Cette classe représente un fichier Apple Archive (.aar). Utilisez‑la pour composer des fichiers Apple Archive.

```csharp
public class AppleArchive : IArchive
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [AppleArchive](applearchive/#constructor)(AppleArchiveEntrySettings) | Initialise une nouvelle instance de la classe `AppleArchive` avec les paramètres utilisés pour les entrées composées. |
| [AppleArchive](applearchive/#constructor_1)(Stream, AppleArchiveLoadOptions) | Initialise une nouvelle instance de la classe `AppleArchive` et compose une liste d'entrées pouvant être extraites de l'archive. |
| [AppleArchive](applearchive/#constructor_2)(string, AppleArchiveLoadOptions) | Initialise une nouvelle instance de la classe `AppleArchive` et compose une liste d'entrées pouvant être extraites de l'archive. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Entries](../../aspose.zip.apple/applearchive/entries/) { get; } | Obtient les entrées constituant l'archive. |
| [IsSolid](../../aspose.zip.apple/applearchive/issolid/) { get; } | Obtient une valeur indiquant si l'archive utilise la compression solide. En mode solide, toutes les données des entrées sont compressées en un seul flux et l'extraction individuelle des entrées n'est pas disponible. Utilisez [`ExtractToDirectory`](../../aspose.zip/iarchive/extracttodirectory/) à la place. |
| [NewEntrySettings](../../aspose.zip.apple/applearchive/newentrysettings/) { get; } | Obtient les paramètres utilisés pour les nouvelles entrées composées. |

## Méthodes

| Nom | Description |
| --- | --- |
| [CreateEntries](../../aspose.zip.apple/applearchive/createentries/)(DirectoryInfo, bool) | Ajoute à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire indiqué. |
| [CreateEntry](../../aspose.zip.apple/applearchive/createentry/#createentry_1)(string, Stream) | Crée une entrée unique dans l'archive. |
| [CreateEntry](../../aspose.zip.apple/applearchive/createentry/#createentry)(string, FileInfo, bool) | Crée une entrée unique dans l'archive. |
| [CreateEntry](../../aspose.zip.apple/applearchive/createentry/#createentry_2)(string, string, bool) | Crée une entrée unique dans l'archive. |
| [Dispose](../../aspose.zip.apple/applearchive/dispose/)() | Effectue les tâches définies par l'application associées à la libération, la remise ou la réinitialisation des ressources non gérées. |
| [ExtractToDirectory](../../aspose.zip.apple/applearchive/extracttodirectory/)(string) | Extrait tous les fichiers de l'archive vers le répertoire fourni. |
| [Save](../../aspose.zip.apple/applearchive/save/#save)(Stream) | Enregistre l'archive dans le flux fourni. |
| [Save](../../aspose.zip.apple/applearchive/save/#save_1)(string) | Enregistre l'archive dans le fichier de destination fourni. |

## Remarques

Apple et Apple Archive sont des marques déposées d'Apple Inc.

### Voir aussi

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Apple](../../aspose.zip.apple/)
* assembly [Aspose.Zip](../../)


