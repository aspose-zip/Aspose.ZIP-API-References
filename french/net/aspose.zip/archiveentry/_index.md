---
title: Class ArchiveEntry
second_title: Référence de l'API Aspose.ZIP pour .NET
description: Aspose.Zip.ArchiveEntry classe. Représente un seul fichier dans larchive.
type: docs
weight: 20
url: /fr/net/aspose.zip/archiveentry/
---
## ArchiveEntry class

Représente un seul fichier dans l'archive.

```csharp
public abstract class ArchiveEntry : IArchiveFileEntry
```

## Propriétés

| Nom | La description |
| --- | --- |
| [Comment](../../aspose.zip/archiveentry/comment/) { get; } | Obtient le commentaire de l'entrée dans l'archive. |
| [CompressedSize](../../aspose.zip/archiveentry/compressedsize/) { get; } | Obtient la taille du fichier compressé. |
| [CompressionSettings](../../aspose.zip/archiveentry/compressionsettings/) { get; } | Obtient les paramètres de compression ou de décompression. |
| [IsDirectory](../../aspose.zip/archiveentry/isdirectory/) { get; } | Obtient une valeur indiquant si l'entrée représente le répertoire. |
| [ModificationTime](../../aspose.zip/archiveentry/modificationtime/) { get; set; } | Obtient ou définit la date et l'heure de la dernière modification. |
| [Name](../../aspose.zip/archiveentry/name/) { get; } | Obtient le nom de l'entrée dans l'archive. |
| [UncompressedSize](../../aspose.zip/archiveentry/uncompressedsize/) { get; } | Obtient la taille du fichier d'origine. |

## Méthodes

| Nom | La description |
| --- | --- |
| [Extract](../../aspose.zip/archiveentry/extract/#extract_1)(Stream, string) | Extrait l'entrée du flux fourni. |
| [Extract](../../aspose.zip/archiveentry/extract/#extract)(string, string) | Extrait l'entrée du système de fichiers par le chemin fourni. |
| [Open](../../aspose.zip/archiveentry/open/)(string) | Ouvre l'entrée pour extraction et fournit un flux avec un contenu d'entrée décompressé. |

## Événements

| Nom | La description |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip/archiveentry/compressionprogressed/) | Se déclenche lorsqu'une partie du flux brut est compressée. |
| event [ExtractionProgressed](../../aspose.zip/archiveentry/extractionprogressed/) | Se déclenche lorsqu'une partie du flux brut est extraite. |

### Remarques

Jeter un`ArchiveEntry` exemple à[`ArchiveEntryEncrypted`](../archiveentryencrypted/) pour déterminer si l'entrée est cryptée ou non.

### Voir également

* interface [IArchiveFileEntry](../iarchivefileentry/)
* espace de noms [Aspose.Zip](../../aspose.zip/)
* Assemblée [Aspose.Zip](../../)


