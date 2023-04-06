---
title: Class WimDirectoryEntry
second_title: Référence de l'API Aspose.ZIP pour .NET
description: Aspose.Zip.Wim.WimDirectoryEntry classe. Représente un répertoire unique dans larchive wim.
type: docs
weight: 770
url: /fr/net/aspose.zip.wim/wimdirectoryentry/
---
## WimDirectoryEntry class

Représente un répertoire unique dans l'archive wim.

```csharp
public sealed class WimDirectoryEntry : WimEntry
```

## Propriétés

| Nom | La description |
| --- | --- |
| [AllEntries](../../aspose.zip.wim/wimdirectoryentry/allentries/) { get; } | Obtient toutes les entrées de[`WimEntry`](../wimentry/) type constituant le répertoire de manière récursive. |
| [AlternateDataStreams](../../aspose.zip.wim/wimentry/alternatedatastreams/) { get; } | Obtient les noms des flux de données alternatifs pour un fichier ou un répertoire. |
| [Archive](../../aspose.zip.wim/wimentry/archive/) { get; } | Obtient l'archive à laquelle appartient l'entrée. |
| [ChangeTime](../../aspose.zip.wim/wimentry/changetime/) { get; } | Obtient la dernière fois que le fichier ou le répertoire a été modifié. |
| [CreationTime](../../aspose.zip.wim/wimentry/creationtime/) { get; } | Obtient l'heure de création du fichier ou du répertoire. |
| [Directories](../../aspose.zip.wim/wimdirectoryentry/directories/) { get; } | Obtient les entrées de`WimDirectoryEntry` type constituant le répertoire. |
| [FileAttributes](../../aspose.zip.wim/wimentry/fileattributes/) { get; } | Obtient les attributs de fichier ou de répertoire. |
| [Files](../../aspose.zip.wim/wimdirectoryentry/files/) { get; } | Obtient les entrées de[`WimFileEntry`](../wimfileentry/) type constituant le répertoire. |
| [FilesAndDirectories](../../aspose.zip.wim/wimdirectoryentry/filesanddirectories/) { get; } | Obtient les entrées de[`WimEntry`](../wimentry/) type constituant le répertoire. |
| [FullPath](../../aspose.zip.wim/wimentry/fullpath/) { get; } | Obtient le chemin complet de l'entrée dans l'image. |
| [HardLink](../../aspose.zip.wim/wimentry/hardlink/) { get; } | Obtient l'identifiant du lien physique du fichier ou du répertoire. |
| [HasHardLinks](../../aspose.zip.wim/wimentry/hashardlinks/) { get; } | Obtient si le fichier ou le répertoire est connu sous d'autres noms. |
| [Image](../../aspose.zip.wim/wimentry/image/) { get; } | Obtient l'image à laquelle appartient l'entrée. |
| [IsDirectory](../../aspose.zip.wim/wimentry/isdirectory/) { get; } | Obtient une valeur indiquant si l'entrée représente le répertoire. |
| [LastAccessTime](../../aspose.zip.wim/wimentry/lastaccesstime/) { get; } | Obtient l'heure du dernier accès au fichier ou au répertoire. |
| [LastWriteTime](../../aspose.zip.wim/wimentry/lastwritetime/) { get; } | Obtient l'heure de modification du fichier ou du répertoire. |
| [Name](../../aspose.zip.wim/wimentry/name/) { get; } | Obtient le nom de l'entrée dans l'image. |
| [Parent](../../aspose.zip.wim/wimentry/parent/) { get; } | Obtient le répertoire parent auquel appartient l'entrée. |
| [ShortName](../../aspose.zip.wim/wimentry/shortname/) { get; } | Obtient le nom abrégé de l'entrée dans l'image. |

## Méthodes

| Nom | La description |
| --- | --- |
| [ExtractToDirectory](../../aspose.zip.wim/wimdirectoryentry/extracttodirectory/)(string) | Extrait tous les fichiers du répertoire courant vers le répertoire fourni. |
| override [ToString](../../aspose.zip.wim/wimentry/tostring/)() |  |

### Voir également

* class [WimEntry](../wimentry/)
* espace de noms [Aspose.Zip.Wim](../../aspose.zip.wim/)
* Assemblée [Aspose.Zip](../../)


