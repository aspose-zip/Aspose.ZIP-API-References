---
title: Class SevenZipArchiveEntry
second_title: Référence de l'API Aspose.ZIP pour .NET
description: Aspose.Zip.SevenZip.SevenZipArchiveEntry classe. Représente un seul fichier dans larchive 7z.
type: docs
weight: 670
url: /fr/net/aspose.zip.sevenzip/sevenziparchiveentry/
---
## SevenZipArchiveEntry class

Représente un seul fichier dans l'archive 7z.

```csharp
public abstract class SevenZipArchiveEntry : IArchiveFileEntry
```

## Propriétés

| Nom | La description |
| --- | --- |
| [CompressedSize](../../aspose.zip.sevenzip/sevenziparchiveentry/compressedsize/) { get; } | Obtient la taille du fichier compressé. |
| [CompressionSettings](../../aspose.zip.sevenzip/sevenziparchiveentry/compressionsettings/) { get; } | Obtient les paramètres de compression ou de décompression. |
| [IsDirectory](../../aspose.zip.sevenzip/sevenziparchiveentry/isdirectory/) { get; } | Obtient une valeur indiquant si l'entrée représente le répertoire. |
| [ModificationTime](../../aspose.zip.sevenzip/sevenziparchiveentry/modificationtime/) { get; } | Obtient la date et l'heure de la dernière modification. |
| [Name](../../aspose.zip.sevenzip/sevenziparchiveentry/name/) { get; } | Obtient le nom de l'entrée dans l'archive. |
| [UncompressedSize](../../aspose.zip.sevenzip/sevenziparchiveentry/uncompressedsize/) { get; } | Obtient la taille du fichier d'origine. |

## Méthodes

| Nom | La description |
| --- | --- |
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/#extract_1)(Stream, string) | Extrait l'entrée du flux fourni. |
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/#extract)(string, string) | Extrait l'entrée du système de fichiers par le chemin fourni. |
| [Open](../../aspose.zip.sevenzip/sevenziparchiveentry/open/)(string) | Ouvre l'entrée pour l'extraction et fournit un flux avec le contenu de l'entrée. |

## Événements

| Nom | La description |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip.sevenzip/sevenziparchiveentry/compressionprogressed/) | Se déclenche lorsqu'une partie du flux brut est compressée. |

### Remarques

Jeter un`SevenZipArchiveEntry` exemple à[`SevenZipArchiveEntryEncrypted`](../sevenziparchiveentryencrypted/) pour déterminer si l'entrée est cryptée ou non.

### Voir également

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* espace de noms [Aspose.Zip.SevenZip](../../aspose.zip.sevenzip/)
* Assemblée [Aspose.Zip](../../)


