---
title: Class ArchiveEntryEncrypted
second_title: Référence de l'API Aspose.ZIP pour .NET
description: Aspose.Zip.ArchiveEntryEncrypted classe. Entrée Zip qui doit être compressée avec chiffrement ou décompressée avec déchiffrement.
type: docs
weight: 30
url: /fr/net/aspose.zip/archiveentryencrypted/
---
## ArchiveEntryEncrypted class

Entrée Zip qui doit être compressée avec chiffrement ou décompressée avec déchiffrement.

```csharp
public sealed class ArchiveEntryEncrypted : ArchiveEntry
```

## Propriétés

| Nom | La description |
| --- | --- |
| [Comment](../../aspose.zip/archiveentry/comment/) { get; } | Obtient le commentaire de l'entrée dans l'archive. |
| [CompressedSize](../../aspose.zip/archiveentry/compressedsize/) { get; } | Obtient la taille du fichier compressé. |
| [CompressionSettings](../../aspose.zip/archiveentry/compressionsettings/) { get; } | Obtient les paramètres de compression ou de décompression. |
| [EncryptionSettings](../../aspose.zip/archiveentryencrypted/encryptionsettings/) { get; } | Obtient les paramètres de chiffrement ou de déchiffrement. |
| [IsDirectory](../../aspose.zip/archiveentry/isdirectory/) { get; } | Obtient une valeur indiquant si l'entrée représente le répertoire. |
| [ModificationTime](../../aspose.zip/archiveentry/modificationtime/) { get; set; } | Obtient ou définit la date et l'heure de la dernière modification. |
| [Name](../../aspose.zip/archiveentry/name/) { get; } | Obtient le nom de l'entrée dans l'archive. |
| [UncompressedSize](../../aspose.zip/archiveentry/uncompressedsize/) { get; } | Obtient la taille du fichier d'origine. |

## Méthodes

| Nom | La description |
| --- | --- |
| [Extract](../../aspose.zip/archiveentry/extract/)(Stream, string) | Extrait l'entrée du flux fourni. |
| [Extract](../../aspose.zip/archiveentry/extract/)(string, string) | Extrait l'entrée du système de fichiers par le chemin fourni. |
| [Open](../../aspose.zip/archiveentry/open/)(string) | Ouvre l'entrée pour extraction et fournit un flux avec un contenu d'entrée décompressé. |

## Événements

| Nom | La description |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip/archiveentry/compressionprogressed/) | Se déclenche lorsqu'une partie du flux brut est compressée. |
| event [ExtractionProgressed](../../aspose.zip/archiveentry/extractionprogressed/) | Se déclenche lorsqu'une partie du flux brut est extraite. |

### Voir également

* class [ArchiveEntry](../archiveentry/)
* espace de noms [Aspose.Zip](../../aspose.zip/)
* Assemblée [Aspose.Zip](../../)


