---
title: Class TarArchive
second_title: Référence de l'API Aspose.ZIP pour .NET
description: Aspose.Zip.Tar.TarArchive classe. Cette classe représente le fichier darchive tar. Utilisezle pour composer extraire ou mettre à jour des archives tar.
type: docs
weight: 730
url: /fr/net/aspose.zip.tar/tararchive/
---
## TarArchive class

Cette classe représente le fichier d'archive tar. Utilisez-le pour composer, extraire ou mettre à jour des archives tar.

```csharp
public class TarArchive : IArchive
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [TarArchive](tararchive/#constructor)() | Initialise une nouvelle instance du`TarArchive` classe. |
| [TarArchive](tararchive/#constructor_1)(Stream) | Initialise une nouvelle instance du[`Archive`](../../aspose.zip/archive/) la liste des entrées de classe et de composition peut être extraite de l'archive. |
| [TarArchive](tararchive/#constructor_2)(string) | Initialise une nouvelle instance du`TarArchive` la liste des entrées de classe et de composition peut être extraite de l'archive. |

## Propriétés

| Nom | La description |
| --- | --- |
| [Entries](../../aspose.zip.tar/tararchive/entries/) { get; } | Obtient les entrées de[`TarEntry`](../tarentry/) type constituant l'archive. |

## Méthodes

| Nom | La description |
| --- | --- |
| static [FromGZip](../../aspose.zip.tar/tararchive/fromgzip/#fromgzip)(Stream) | Extrait l'archive gzip fournie et compose`TarArchive` à partir des données extraites. |
| static [FromGZip](../../aspose.zip.tar/tararchive/fromgzip/#fromgzip_1)(string) | Extrait l'archive gzip fournie et compose`TarArchive` à partir des données extraites. |
| static [FromLZip](../../aspose.zip.tar/tararchive/fromlzip/#fromlzip)(Stream) | Extrait l'archive lzip fournie et compose`TarArchive` à partir des données extraites. |
| static [FromLZip](../../aspose.zip.tar/tararchive/fromlzip/#fromlzip_1)(string) | Extrait l'archive lzip fournie et compose`TarArchive` à partir des données extraites. |
| static [FromXz](../../aspose.zip.tar/tararchive/fromxz/#fromxz)(Stream) | Extrait l'archive au format xz fournie et compose`TarArchive` à partir des données extraites. |
| static [FromXz](../../aspose.zip.tar/tararchive/fromxz/#fromxz_1)(string) | Extrait l'archive au format xz fournie et compose`TarArchive` à partir des données extraites. |
| static [FromZ](../../aspose.zip.tar/tararchive/fromz/#fromz)(Stream) | Extrait l'archive au format Z fournie et compose`TarArchive` à partir des données extraites. |
| static [FromZ](../../aspose.zip.tar/tararchive/fromz/#fromz_1)(string) | Extrait l'archive au format Z fournie et compose`TarArchive` à partir des données extraites. |
| [CreateEntries](../../aspose.zip.tar/tararchive/createentries/#createentries)(DirectoryInfo, bool) | Ajoute à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire donné. |
| [CreateEntries](../../aspose.zip.tar/tararchive/createentries/#createentries_1)(string, bool) | Ajoute à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire donné. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry/#createentry)(string, FileInfo, bool) | Créer une entrée unique dans l'archive. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry/#createentry_1)(string, Stream, FileSystemInfo) | Créer une entrée unique dans l'archive. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry/#createentry_2)(string, string, bool) | Créer une entrée unique dans l'archive. |
| [DeleteEntry](../../aspose.zip.tar/tararchive/deleteentry/#deleteentry_1)(int) | Supprime l'entrée de la liste des entrées par index. |
| [DeleteEntry](../../aspose.zip.tar/tararchive/deleteentry/#deleteentry)(TarEntry) | Supprime la première occurrence d'une entrée spécifique de la liste des entrées. |
| [Dispose](../../aspose.zip.tar/tararchive/dispose/)() | Effectue des tâches définies par l'application associées à la libération, à la libération ou à la réinitialisation des ressources non gérées. |
| [ExtractToDirectory](../../aspose.zip.tar/tararchive/extracttodirectory/)(string) | Extrait tous les fichiers de l'archive dans le répertoire fourni. |
| [Save](../../aspose.zip.tar/tararchive/save/#save)(Stream, TarFormat?) | Enregistre l'archive dans le flux fourni. |
| [Save](../../aspose.zip.tar/tararchive/save/#save_1)(string, TarFormat?) | Enregistre l'archive dans le fichier de destination fourni. |
| [SaveGzipped](../../aspose.zip.tar/tararchive/savegzipped/#savegzipped)(Stream, TarFormat?) | Enregistre l'archive dans le flux avec compression gzip. |
| [SaveGzipped](../../aspose.zip.tar/tararchive/savegzipped/#savegzipped_1)(string, TarFormat?) | Enregistre l'archive dans le fichier par chemin avec compression gzip. |
| [SaveLzipped](../../aspose.zip.tar/tararchive/savelzipped/#savelzipped)(Stream, TarFormat?) | Enregistre l'archive dans le flux avec la compression lzip. |
| [SaveLzipped](../../aspose.zip.tar/tararchive/savelzipped/#savelzipped_1)(string, TarFormat?) | Enregistre l'archive dans le fichier par chemin avec compression lzip. |
| [SaveXzCompressed](../../aspose.zip.tar/tararchive/savexzcompressed/#savexzcompressed)(Stream, TarFormat?, XzArchiveSettings) | Enregistre l'archive dans le flux avec une compression xz. |
| [SaveXzCompressed](../../aspose.zip.tar/tararchive/savexzcompressed/#savexzcompressed_1)(string, TarFormat?, XzArchiveSettings) | Enregistre l'archive dans le chemin par chemin avec une compression xz. |
| [SaveZCompressed](../../aspose.zip.tar/tararchive/savezcompressed/#savezcompressed)(Stream, TarFormat?) | Enregistre l'archive dans le flux avec compression Z. |
| [SaveZCompressed](../../aspose.zip.tar/tararchive/savezcompressed/#savezcompressed_1)(string, TarFormat?) | Enregistre l'archive dans le chemin par chemin avec la compression Z. |

### Voir également

* interface [IArchive](../../aspose.zip/iarchive/)
* espace de noms [Aspose.Zip.Tar](../../aspose.zip.tar/)
* Assemblée [Aspose.Zip](../../)


