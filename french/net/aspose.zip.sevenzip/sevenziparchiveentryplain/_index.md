---
title: Class SevenZipArchiveEntryPlain
second_title: Référence de l'API Aspose.ZIP pour .NET
description: Aspose.Zip.SevenZip.SevenZipArchiveEntryPlain classe. Entrée SevenZip qui doit être compressée sans chiffrement ou décompressée sans déchiffrement.
type: docs
weight: 690
url: /fr/net/aspose.zip.sevenzip/sevenziparchiveentryplain/
---
## SevenZipArchiveEntryPlain class

Entrée SevenZip qui doit être compressée sans chiffrement ou décompressée sans déchiffrement.

```csharp
public class SevenZipArchiveEntryPlain : SevenZipArchiveEntry
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
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/)(Stream, string) | Extrait l'entrée du flux fourni. |
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/)(string, string) | Extrait l'entrée du système de fichiers par le chemin fourni. |
| [Open](../../aspose.zip.sevenzip/sevenziparchiveentry/open/)(string) | Ouvre l'entrée pour l'extraction et fournit un flux avec le contenu de l'entrée. |

## Événements

| Nom | La description |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip.sevenzip/sevenziparchiveentry/compressionprogressed/) | Se déclenche lorsqu'une partie du flux brut est compressée. |

### Voir également

* class [SevenZipArchiveEntry](../sevenziparchiveentry/)
* espace de noms [Aspose.Zip.SevenZip](../../aspose.zip.sevenzip/)
* Assemblée [Aspose.Zip](../../)


