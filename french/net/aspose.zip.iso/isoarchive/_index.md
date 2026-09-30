---
title: "Classe IsoArchive"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Classe Aspose.Zip.Iso.IsoArchive. Représente une archive ISO ISO 9660"
type: docs
weight: 570
url: /fr/net/aspose.zip.iso/isoarchive/
---
## IsoArchive class

Représente une archive ISO (ISO 9660).

```csharp
public sealed class IsoArchive : IArchive
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [IsoArchive](isoarchive/#constructor)() | Initialise une nouvelle instance de la classe `IsoArchive` et crée une archive ISO vide pour ajouter de nouveaux fichiers et répertoires. |
| [IsoArchive](isoarchive/#constructor_1)(Stream, IsoLoadOptions) | Initialise une nouvelle instance de la classe `IsoArchive` et compose une liste d'entrées qui peut être extraite de l'archive. |
| [IsoArchive](isoarchive/#constructor_2)(string, IsoLoadOptions) | Initialise une nouvelle instance de la classe `IsoArchive` et compose une liste d'entrées qui peut être extraite de l'archive. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Entries](../../aspose.zip.iso/isoarchive/entries/) { get; } | Obtient les entrées de type [`IsoEntry`](../isoentry/) constituant l'archive. |

## Méthodes

| Nom | Description |
| --- | --- |
| [CreateDirectory](../../aspose.zip.iso/isoarchive/createdirectory/)(string) | Ajoute un répertoire à l'image ISO. |
| [CreateEntry](../../aspose.zip.iso/isoarchive/createentry/#createentry)(string) | Ajoute un fichier à l'image ISO. |
| [CreateEntry](../../aspose.zip.iso/isoarchive/createentry/#createentry_1)(string, Stream) | Ajoute un fichier à l'image ISO. |
| [CreateEntry](../../aspose.zip.iso/isoarchive/createentry/#createentry_2)(string, string) | Ajoute un fichier à l'image ISO. |
| [Dispose](../../aspose.zip.iso/isoarchive/dispose/)() | Effectue les tâches définies par l'application associées à la libération, la remise ou la réinitialisation des ressources non gérées. |
| [ExtractToDirectory](../../aspose.zip.iso/isoarchive/extracttodirectory/)(string) | Extrait toutes les entrées vers le répertoire spécifié. |
| [Save](../../aspose.zip.iso/isoarchive/save/#save)(Stream, IsoSaveOptions) | Enregistre l'image ISO dans le flux spécifié. |
| [Save](../../aspose.zip.iso/isoarchive/save/#save_1)(string, IsoSaveOptions) | Enregistre l'image ISO dans le chemin spécifié. |

### Voir aussi

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Iso](../../aspose.zip.iso/)
* assembly [Aspose.Zip](../../)


