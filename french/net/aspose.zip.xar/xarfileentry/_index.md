---
title: Class XarFileEntry
second_title: Référence de l'API Aspose.ZIP pour .NET
description: Aspose.Zip.Xar.XarFileEntry classe. Représente lentrée de fichier dans larchive xar.
type: docs
weight: 840
url: /fr/net/aspose.zip.xar/xarfileentry/
---
## XarFileEntry class

Représente l'entrée de fichier dans l'archive xar.

```csharp
public abstract class XarFileEntry : XarEntry, IArchiveFileEntry
```

## Propriétés

| Nom | La description |
| --- | --- |
| [CreationTime](../../aspose.zip.xar/xarentry/creationtime/) { get; } | Obtient l'heure de création du fichier ou du répertoire. |
| [FullPath](../../aspose.zip.xar/xarentry/fullpath/) { get; } | Obtient le chemin complet de l'entrée dans l'archive. |
| [IsDirectory](../../aspose.zip.xar/xarentry/isdirectory/) { get; } | Obtient une valeur indiquant si l'entrée représente le répertoire. |
| [LastAccessTime](../../aspose.zip.xar/xarentry/lastaccesstime/) { get; } | Obtient l'heure du dernier accès au fichier ou au répertoire. |
| [LastWriteTime](../../aspose.zip.xar/xarentry/lastwritetime/) { get; } | Obtient l'heure de modification du fichier ou du répertoire. |
| abstract [Length](../../aspose.zip.xar/xarfileentry/length/) { get; } | Obtient la longueur de l'entrée en octets. |
| [Name](../../aspose.zip.xar/xarentry/name/) { get; } | Obtient le nom de l'entrée dans l'archive. |
| [Parent](../../aspose.zip.xar/xarentry/parent/) { get; } | Obtient le répertoire parent auquel appartient l'entrée. |

## Méthodes

| Nom | La description |
| --- | --- |
| abstract [Extract](../../aspose.zip.xar/xarfileentry/extract/#extract_1)(Stream) | Extrait l'entrée du flux fourni. |
| abstract [Extract](../../aspose.zip.xar/xarfileentry/extract/#extract)(string) | Extrait l'entrée du système de fichiers par le chemin fourni. |
| abstract [Open](../../aspose.zip.xar/xarfileentry/open/)() | Ouvre l'entrée pour l'extraction et fournit un flux avec le contenu de l'entrée. |
| override [ToString](../../aspose.zip.xar/xarentry/tostring/)() |  |

### Voir également

* class [XarEntry](../xarentry/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* espace de noms [Aspose.Zip.Xar](../../aspose.zip.xar/)
* Assemblée [Aspose.Zip](../../)


