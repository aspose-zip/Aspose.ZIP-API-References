---
title: Class CpioArchive
second_title: Référence de l'API Aspose.ZIP pour .NET
description: Aspose.Zip.Cpio.CpioArchive classe. Cette classe représente le fichier darchive cpio.
type: docs
weight: 160
url: /fr/net/aspose.zip.cpio/cpioarchive/
---
## CpioArchive class

Cette classe représente le fichier d'archive cpio.

```csharp
public class CpioArchive : IArchive
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [CpioArchive](cpioarchive/#constructor)() | Initialise une nouvelle instance du`CpioArchive` classe. |
| [CpioArchive](cpioarchive/#constructor_1)(Stream) | Initialise une nouvelle instance du`CpioArchive` la liste des entrées de classe et de composition peut être extraite de l'archive. |
| [CpioArchive](cpioarchive/#constructor_2)(string) | Initialise une nouvelle instance du`CpioArchive` la liste des entrées de classe et de composition peut être extraite de l'archive. |

## Propriétés

| Nom | La description |
| --- | --- |
| [Entries](../../aspose.zip.cpio/cpioarchive/entries/) { get; } | Obtient les entrées de[`CpioEntry`](../cpioentry/) type constituant l'archive. |

## Méthodes

| Nom | La description |
| --- | --- |
| [CreateEntries](../../aspose.zip.cpio/cpioarchive/createentries/#createentries)(DirectoryInfo, bool) | Ajoute à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire donné. |
| [CreateEntries](../../aspose.zip.cpio/cpioarchive/createentries/#createentries_1)(string, bool) | Ajoute à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire donné. |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry_1)(string, Stream) | Créer une entrée unique dans l'archive. |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry)(string, FileInfo, bool) | Créer une entrée unique dans l'archive. |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry_2)(string, string, bool) | Créer une entrée unique dans l'archive. |
| [DeleteEntry](../../aspose.zip.cpio/cpioarchive/deleteentry/#deleteentry)(CpioEntry) | Supprime la première occurrence d'une entrée spécifique de la liste des entrées. |
| [DeleteEntry](../../aspose.zip.cpio/cpioarchive/deleteentry/#deleteentry_1)(int) | Supprime l'entrée de la liste des entrées par index. |
| [Dispose](../../aspose.zip.cpio/cpioarchive/dispose/)() | Effectue des tâches définies par l'application associées à la libération, à la libération ou à la réinitialisation des ressources non gérées. |
| [ExtractToDirectory](../../aspose.zip.cpio/cpioarchive/extracttodirectory/)(string) | Extrait tous les fichiers de l'archive dans le répertoire fourni. |
| [Save](../../aspose.zip.cpio/cpioarchive/save/#save)(Stream, CpioFormat) | Enregistre l'archive dans le flux fourni. |
| [Save](../../aspose.zip.cpio/cpioarchive/save/#save_1)(string, CpioFormat) | Enregistre l'archive dans le fichier de destination fourni. |
| [SaveGzipped](../../aspose.zip.cpio/cpioarchive/savegzipped/#savegzipped)(Stream, CpioFormat) | Enregistre l'archive dans le flux avec compression gzip. |
| [SaveGzipped](../../aspose.zip.cpio/cpioarchive/savegzipped/#savegzipped_1)(string, CpioFormat) | Enregistre l'archive dans le fichier par chemin avec compression gzip. |
| [SaveXzCompressed](../../aspose.zip.cpio/cpioarchive/savexzcompressed/#savexzcompressed)(Stream, CpioFormat, XzArchiveSettings) | Enregistre l'archive dans le flux avec une compression xz. |
| [SaveXzCompressed](../../aspose.zip.cpio/cpioarchive/savexzcompressed/#savexzcompressed_1)(string, CpioFormat, XzArchiveSettings) | Enregistre l'archive dans le chemin par chemin avec une compression xz. |

### Voir également

* interface [IArchive](../../aspose.zip/iarchive/)
* espace de noms [Aspose.Zip.Cpio](../../aspose.zip.cpio/)
* Assemblée [Aspose.Zip](../../)


