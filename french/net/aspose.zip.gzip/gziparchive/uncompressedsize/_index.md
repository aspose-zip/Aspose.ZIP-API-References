---
title: "GzipArchive.UncompressedSize"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Propriété GzipArchive. Obtient la taille d'un fichier original."
type: docs
weight: 30
url: /fr/net/aspose.zip.gzip/gziparchive/uncompressedsize/
---
## GzipArchive.UncompressedSize property

Obtient la taille d'un fichier original.

```csharp
public ulong UncompressedSize { get; }
```

### Exceptions

| exception | condition |
| --- | --- |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |

## Remarques

Lors de la décompression, cette propriété peut contenir une taille incorrecte. Si la taille du fichier décompressé dépasse 4 Go, cette propriété donnera une valeur erronée en raison de la limite de 32 bits dans l'en-tête.

### Voir aussi

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)


