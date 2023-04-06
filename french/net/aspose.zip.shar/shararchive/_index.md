---
title: Class SharArchive
second_title: Référence de l'API Aspose.ZIP pour .NET
description: Aspose.Zip.Shar.SharArchive classe. Cette classe représente le fichier darchive partagé.
type: docs
weight: 700
url: /fr/net/aspose.zip.shar/shararchive/
---
## SharArchive class

Cette classe représente le fichier d'archive partagé.

```csharp
public class SharArchive : IDisposable
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [SharArchive](shararchive/#constructor)() | Initialise une nouvelle instance du`SharArchive` classe. |
| [SharArchive](shararchive/#constructor_1)(string) |  |

## Propriétés

| Nom | La description |
| --- | --- |
| [Entries](../../aspose.zip.shar/shararchive/entries/) { get; } | Obtient les entrées de[`SharEntry`](../sharentry/) type constituant l'archive. |

## Méthodes

| Nom | La description |
| --- | --- |
| [CreateEntries](../../aspose.zip.shar/shararchive/createentries/#createentries)(DirectoryInfo, bool) | Ajoute à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire donné. |
| [CreateEntries](../../aspose.zip.shar/shararchive/createentries/#createentries_1)(string, bool) | Ajoute à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire donné. |
| [CreateEntry](../../aspose.zip.shar/shararchive/createentry/#createentry_1)(string, Stream) | Créer une entrée unique dans l'archive. |
| [CreateEntry](../../aspose.zip.shar/shararchive/createentry/#createentry)(string, FileInfo, bool) | Créer une entrée unique dans l'archive. |
| [CreateEntry](../../aspose.zip.shar/shararchive/createentry/#createentry_2)(string, string, bool) | Créer une entrée unique dans l'archive. |
| [DeleteEntry](../../aspose.zip.shar/shararchive/deleteentry/#deleteentry_1)(int) | Supprime l'entrée de la liste des entrées par index. |
| [DeleteEntry](../../aspose.zip.shar/shararchive/deleteentry/#deleteentry)(SharEntry) | Supprime la première occurrence d'une entrée spécifique de la liste des entrées. |
| [Dispose](../../aspose.zip.shar/shararchive/dispose/)() | Effectue des tâches définies par l'application associées à la libération, à la libération ou à la réinitialisation des ressources non gérées. |
| [Save](../../aspose.zip.shar/shararchive/save/#save)(Stream) | Enregistre l'archive dans le flux fourni. |
| [Save](../../aspose.zip.shar/shararchive/save/#save_1)(string) | Enregistre l'archive dans le fichier de destination fourni. |

### Voir également

* espace de noms [Aspose.Zip.Shar](../../aspose.zip.shar/)
* Assemblée [Aspose.Zip](../../)


