---
title: "Classe AlzEntryEncrypted"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Classe Aspose.Zip.Alz.AlzEntryEncrypted. Entrée ALZ qui doit être déchiffrée avant la décompression"
type: docs
weight: 40
url: /fr/net/aspose.zip.alz/alzentryencrypted/
---
## AlzEntryEncrypted class

Entrée ALZ qui doit être décryptée avant la décompression.

```csharp
public sealed class AlzEntryEncrypted : AlzEntry
```

## Propriétés

| Nom | Description |
| --- | --- |
| [CompressedSize](../../aspose.zip.alz/alzentry/compressedsize/) { get; } | Taille compressée des données du fichier en octets. |
| [IsDirectory](../../aspose.zip.alz/alzentry/isdirectory/) { get; } | Renvoie true si cette entrée représente un répertoire. |
| [Length](../../aspose.zip.alz/alzentry/length/) { get; } |  |
| [Name](../../aspose.zip.alz/alzentry/name/) { get; } | Nom de fichier (sans le chemin). |
| [UncompressedSize](../../aspose.zip.alz/alzentry/uncompressedsize/) { get; } | Taille décompressée des données du fichier en octets. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Extract](../../aspose.zip.alz/alzentry/extract/)(Stream, string) | Extrait l'entrée vers le flux fourni. |
| [Extract](../../aspose.zip.alz/alzentry/extract/)(string, string) | Extrait l'entrée dans le système de fichiers au chemin fourni. |
| [Open](../../aspose.zip.alz/alzentry/open/)(string) | Ouvre l'entrée pour l'extraction et fournit un flux avec le contenu décompressé de l'entrée. |

### Voir aussi

* class [AlzEntry](../alzentry/)
* namespace [Aspose.Zip.Alz](../../aspose.zip.alz/)
* assembly [Aspose.Zip](../../)


