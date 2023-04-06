---
title: Class RarArchiveEntry
second_title: Référence de l'API Aspose.ZIP pour .NET
description: Aspose.Zip.Rar.RarArchiveEntry classe. Représente un seul fichier dans larchive.
type: docs
weight: 320
url: /fr/net/aspose.zip.rar/rararchiveentry/
---
## RarArchiveEntry class

Représente un seul fichier dans l'archive.

```csharp
public abstract class RarArchiveEntry : IArchiveFileEntry
```

## Propriétés

| Nom | La description |
| --- | --- |
| [CompressedSize](../../aspose.zip.rar/rararchiveentry/compressedsize/) { get; } | Obtient la taille du fichier compressé. |
| [CreationTime](../../aspose.zip.rar/rararchiveentry/creationtime/) { get; } | Obtient la date et l'heure de création. |
| [IsDirectory](../../aspose.zip.rar/rararchiveentry/isdirectory/) { get; } | Obtient une valeur indiquant si l'entrée représente le répertoire. |
| [LastAccessTime](../../aspose.zip.rar/rararchiveentry/lastaccesstime/) { get; } | Obtient la date et l'heure du dernier accès. |
| [ModificationTime](../../aspose.zip.rar/rararchiveentry/modificationtime/) { get; } | Obtient la date et l'heure de la dernière modification. |
| [Name](../../aspose.zip.rar/rararchiveentry/name/) { get; } | Obtient le nom de l'entrée dans l'archive. |
| [UncompressedSize](../../aspose.zip.rar/rararchiveentry/uncompressedsize/) { get; } | Obtient la taille du fichier d'origine. |

## Méthodes

| Nom | La description |
| --- | --- |
| [Extract](../../aspose.zip.rar/rararchiveentry/extract/#extract_1)(Stream, string) | Extrait l'entrée du flux fourni. |
| [Extract](../../aspose.zip.rar/rararchiveentry/extract/#extract)(string, string) | Extrait l'entrée du système de fichiers par le chemin fourni. |
| [Open](../../aspose.zip.rar/rararchiveentry/open/)(string) | Ouvre l'entrée pour extraction et fournit un flux avec un contenu d'entrée décompressé. |

## Événements

| Nom | La description |
| --- | --- |
| event [ExtractionProgressed](../../aspose.zip.rar/rararchiveentry/extractionprogressed/) | Se déclenche lorsqu'une partie du flux brut est extraite. |

### Remarques

Lancer un`RarArchiveEntry` exemple à[`RarArchiveEntryEncrypted`](../rararchiveentryencrypted/) pour déterminer si l'entrée est cryptée ou non.

### Voir également

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* espace de noms [Aspose.Zip.Rar](../../aspose.zip.rar/)
* Assemblée [Aspose.Zip](../../)


