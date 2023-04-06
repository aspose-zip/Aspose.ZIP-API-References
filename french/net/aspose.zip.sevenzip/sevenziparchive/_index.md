---
title: Class SevenZipArchive
second_title: Référence de l'API Aspose.ZIP pour .NET
description: Aspose.Zip.SevenZip.SevenZipArchive classe. Cette classe représente le fichier darchive 7z. Utilisezle pour composer et extraire des archives 7z.
type: docs
weight: 660
url: /fr/net/aspose.zip.sevenzip/sevenziparchive/
---
## SevenZipArchive class

Cette classe représente le fichier d'archive 7z. Utilisez-le pour composer et extraire des archives 7z.

```csharp
public class SevenZipArchive : IArchive
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [SevenZipArchive](sevenziparchive/#constructor)(SevenZipEntrySettings) | Initialise une nouvelle instance du`SevenZipArchive` classe avec des paramètres facultatifs pour ses entrées. |
| [SevenZipArchive](sevenziparchive/#constructor_1)(Stream) | Initialise une nouvelle instance du`SevenZipArchive` la liste des entrées de classe et de composition peut être extraite de l'archive. |
| [SevenZipArchive](sevenziparchive/#constructor_2)(string) | Initialise une nouvelle instance du`SevenZipArchive` la liste des entrées de classe et de composition peut être extraite de l'archive. |

## Propriétés

| Nom | La description |
| --- | --- |
| [Entries](../../aspose.zip.sevenzip/sevenziparchive/entries/) { get; } | Obtient les entrées de[`SevenZipArchiveEntry`](../sevenziparchiveentry/) type constituant l'archive. |
| [NewEntrySettings](../../aspose.zip.sevenzip/sevenziparchive/newentrysettings/) { get; } | Paramètres de compression et de chiffrement utilisés pour les nouveaux[`SevenZipArchiveEntry`](../sevenziparchiveentry/) articles. |

## Méthodes

| Nom | La description |
| --- | --- |
| [CreateEntries](../../aspose.zip.sevenzip/sevenziparchive/createentries/#createentries)(DirectoryInfo, bool) | Ajoute à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire donné. |
| [CreateEntries](../../aspose.zip.sevenzip/sevenziparchive/createentries/#createentries_1)(string, bool) | Ajoute à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire donné. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_1)(string, Stream, SevenZipEntrySettings) | Créer une entrée unique dans l'archive. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry)(string, FileInfo, bool, SevenZipEntrySettings) | Créer une entrée unique dans l'archive. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_2)(string, Stream, SevenZipEntrySettings, FileSystemInfo) | Créer une entrée unique dans l'archive. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_3)(string, string, bool, SevenZipEntrySettings) | Créer une entrée unique dans l'archive. |
| [Dispose](../../aspose.zip.sevenzip/sevenziparchive/dispose/)() | Effectue des tâches définies par l'application associées à la libération, à la libération ou à la réinitialisation des ressources non gérées. |
| [ExtractToDirectory](../../aspose.zip.sevenzip/sevenziparchive/extracttodirectory/)(string, string) | Extrait tous les fichiers de l'archive dans le répertoire fourni. |
| [Save](../../aspose.zip.sevenzip/sevenziparchive/save/#save)(Stream) | Enregistre l'archive 7z dans le flux fourni. |
| [Save](../../aspose.zip.sevenzip/sevenziparchive/save/#save_1)(string) | Enregistre l'archive dans le fichier de destination fourni. |
| [SaveSplit](../../aspose.zip.sevenzip/sevenziparchive/savesplit/)(string, SplitSevenZipArchiveSaveOptions) | Enregistre l'archive multi-volume dans le répertoire de destination fourni. |

### Voir également

* interface [IArchive](../../aspose.zip/iarchive/)
* espace de noms [Aspose.Zip.SevenZip](../../aspose.zip.sevenzip/)
* Assemblée [Aspose.Zip](../../)


